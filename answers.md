1. Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead (hint: use attr()).

  $('img.profile-image').attr('src', 'http://placehold.it/400x400')

2. Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing.

  $('#left-image img').attr('src', 'http://cdn3-www.cattime.com/assets/uploads/2011/08/best-kitten-names-1.jpg')

3. Select the heading that says "Panda the Bear" and change it to your own name. (hint: use text())

  $('h1').first().text('Stephanie Wu')

4. Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector)

  $('#employment h3').text('Experience')

5. Panda the Bear is lying about their skills! Take the "time travel" skill off the page to satisfy your personal sense of justice.

  $('#time-travel').parent().remove()

6. Change the colour of the body.

  $('body').css('background-color', 'black')

7. Change the colour used by the highlight class.

  $('.highlight').css('color', 'darkgreen')

8. Change the font family of the h1 to 'monospace'.

  $('h1').css('font-family', 'monospace')

9. Find a way to select the round icons in the sidebar and then change their colour.

  $('.action-icon-bg').css('background-color', 'darkgreen')

10. Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself."

  $('form input').first().attr('placeholder', 'Identify yourself')

11. Give the name field a "value" attribute of "your nemesis".

  $('form input').first().attr('value', 'Your nemesis')

12. Change the value attribute of the email field to "koalathebear@gmail.com".

  $('#email').attr('value', 'koalathebear@gmail.com')

13. Change the value of the submit button on the contact form to "En garde!".

  $('#submit').attr('value', 'En garde!')

14. That drawing of Pikachu is really cute. Let’s duplicate it using clone() and insert it at the bottom of the page using insertAfter() or appendTo().

  $('#right-image img').clone().insertAfter( $('.portfolio-container') )

15. Wow, that was so satisfying I think we should do it 10 more times. Use a for loop to help you do this.

  for (var i = 0; i < 10; i++ ) { $('#right-image img').clone().insertAfter( $('.portfolio-container') ) };

16. Add last updated to page

  var listItem = document.createElement('li');
  var leftSpan = document.createElement('span');
  var lastUpdated = document.createTextNode('Page last updated on');
  leftSpan.appendChild(lastUpdated);
  listItem.appendChild(leftSpan);
  var rightSpan = document.createElement('span');
  var updateDate = document.lastModified;
  var dateNode = document.createTextNode(updateDate);
  rightSpan.appendChild(dateNode);
  listItem.appendChild(rightSpan);

jQuery

  $('ul.bio-info').append(listItem);
