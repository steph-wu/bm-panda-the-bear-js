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
