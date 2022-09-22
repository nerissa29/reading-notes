## Reding Notes 9

### HTML Forms

#### Why are forms so important in web development?
 Forms are used to collect visitor's data; it is "interaction between a user and a web site or application"[^1]. Forms are used to interact with the user, allowing them to enter data, the data will then be sent to the web server for processing or storage. In businesses, it is mainly to use to let the user enter their information when it comes to payment online, or aloows the user to either add lists "or show hide  a feature"[^.1].
 
 #### When designing a form, what are some key things to keep in mind when it comes to user experience?
 
 Mifsud (2011) shared the figured below in his article, translating each "reasons into the user and business objectives that lie behind them"[^2]:
 
 <img width="564" alt="image" src="https://user-images.githubusercontent.com/113204667/191780270-a3b1ef45-0add-42a6-aae5-5f27b0295b1c.png">

Mifsud (2011) also mentioned that[^2]:

- Forms can make a website usable or unusable, because they stand in the way of the user achieving their goal;
- Forms need to be usable in order to help the user achieve that goal.

#### List 5 form elements and explain their importance.

The form elements can contain the following:
- input
  - an inout field where the user can enter his/her data[^3]
- textarea
  - used to collect user inputs, such as reviews or comments[^4]
- button
  - a clickable button with a text (ex. Submit, Cancel, etc.)[^5]
- select
  - a drop-down list of options, mostly used to cllect user input[^6]
 - option 
   - also a drop-down list placed inside the select, datalist, or optgroup element[^7]
 
 ### Introduction To Events.
 
 #### How would you describe events to a non-technical friend?
 
I would describe events to a non-technical friend by breaking the ice and story-telling to give them time to get ready before throwing them technical information. Being attentive, and using visuals to better explain the topic might help.

#### When using the addEventListener() method, what 2 arguments will you need to provide?

The addEventListener can take two arguments, the (1) name of the event and the (2) function handling the event[^8]:

```
const btn = document.querySelector('button');

function random(number) {
  return Math.floor(Math.random() * (number+1));
}

btn.addEventListener('click', () => {
  const rndCol = `rgb(${random(255)}, ${random(255)}, ${random(255)})`;
  document.body.style.backgroundColor = rndCol;
});

```

- the 'click' on the code above, indicates that we are waiting or listening to that click
- the function above generates a random color (RGB) and sets the page's body background color "equal to that color"[^8].

#### Describe the event object. Why is the target within the event object useful?
 
 
 [^1]: [Your first form](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form)
 [^2]: [An Extensive Guide To Web Form Usability](https://www.smashingmagazine.com/2011/11/extensive-guide-web-form-usability
 [^3]: [HTML Input Tag](https://www.w3schools.com/tags/tag_input.asp)
 [^4]: [HTML <textarea> Tag](https://www.w3schools.com/tags/tag_textarea.asp)
 [^5]: [HTML Button Tag](https://www.w3schools.com/tags/tag_button.asp)
 [^6]: [HTML Select Tag](https://www.w3schools.com/tags/tag_select.asp)
 [^7]: [HTML Option Tag](https://www.w3schools.com/tags/tag_option.asp)
 [^8]: [Introduction to events](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)
 
 
