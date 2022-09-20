## Reading Notes 7
## Readings: Object-Oriented Programming, HTML Tables

#### Explain why we need domain modeling.

It is "is the process of creating a conceptual model in code for a specific problem"[^1].
It acts like a vocabulary used in both business an technical teams; it carries out a language and structure critical for the analysis.


#### Why should tables not be used for page layouts?

Tables are use to present data in table form; it is not use for layout

#### List and describe 3 different semantic HTML elements used in an HTML

A semantic element example[^1]:
- *article element* - a self-contained content
- *figcaption* - defines caption for figures
- *aside element* - defines content *aside* from the page's content

## Introducing constructors

#### What is a constructor and what are some advantages to using it?

Constructors name begin with capital letter, and is usually named for the object type they create; a sample shown below is adapated from MDN[^2]:

```
function Person(name) {
  this.name = name;
  this.introduceSelf = function() {
    console.log(`Hi! I'm ${this.name}.`);
  }
}
```
To call the constructor, Person() above[^2]:

```
const salva = new Person('Salva');
salva.name;
salva.introduceSelf();

const frankie = new Person('Frankie');
frankie.name;
frankie.introduceSelf();
```





[^1]: [Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)
[^2]: [JavaScript Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors)



