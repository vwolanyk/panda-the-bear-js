**PANDA SAYS:**

**_Part 1_**

1. profileImage.src = "https://ih1.redbubble.net/image.316783031.6471/flat,400x480,075,f.u1.jpg";

1. var skyImage = document.querySelector('div#left-image.portfolio-image img');

    skyImage.width = 325

2.  var heading = document.querySelector('h1.highlight');

    heading.innerHTML = "The Vladinator";

3. var employmentHeader = document.querySelector("div#employment.info-inner-container h3.info-title");

    employmentHeader.innerText = '\u2620   Experience ';

4. var body = document.querySelector('body');

    body.style.backgroundColor = "brown";

5. var highlight = document.querySelectorAll(".highlight");

    highlight.forEach(function(item){ item.style.color = "yellow";});

6. var h1 = document.querySelectorAll("h1");

    h1.forEach(function(title){ title.style.fontFamily = "monospace"});

7. var roundIcon = document.querySelectorAll("a.action-icon-bg");

    roundIcon.forEach(function(icon){ icon.style.backgroundColor = "purple"; });

8. var nameInput = document.querySelector("input#name.contact-info");

    nameInput.placeholder = "VERIFY Yourself"

9. var messageInput = document.querySelector("textarea#message");

    messageInput.placeholder = "SAY it don't Spray it";

10. nameInput.value  = "My Nemesis"

11. var emailInput = document.querySelector("input#email.contact-info");

    emailInput.value = "koalathebear@gmail.com"

12. var submitButton = document.querySelector("input#submit");

    submitButton.value = "En Garde!";

13. submitButton.disabled = true;

14. var form =  document.querySelector("form");

    form.reset();


_PART 2_

**Removing Elements From DOM**

``
1.  var child = document.querySelectorAll('div.bar-default')[2]

    var parent = document.querySelector('section div')

    parent.removeChild(child)


**Adding Elements to the DOM**


1.  var pikatchu = document.querySelector('div#right-image.portfolio-image img')

    var portfolioContain = document.querySelector('div.portfolio-container')

    portfolioContain.appendChild(pikatchu.cloneNode())


2.  for (i = 0; i < 10; i++) { portfolioContain.appendChild(pikatchu.cloneNode());}


3.  var addListItem = document.createElement('li')

    var bioInfoTitle = document.createElement('span')

          bioInfoTitle.innerText = "Date Last Updated"

          bioInfoTitle.className = "bio-info-title"

    var bioInfoValue = document.createElement('span')

        bioInfoValue.innerHTML = Date();

        bioInfoValue.className = "bio-info-value bio-info-phone"

    addListItem.appendChild(bioInfoTitle)

    addListItem.appendChild(bioInfoValue)

    document.querySelector('ul.bio-info').appendChild(addListItem)
