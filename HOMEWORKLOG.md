Thinking About Expects: koan #2
"It should assert equality a better way."  
This answer uses a function

[expect(actualValue).toEqual(expectedValue)].  

This does work.  Therefore, it is somehow "better" than "expect(actualValue === expectedValue).toBeTruthy();"?  Is this the correct "take-home" message?


### Thinking About Functions
Lexical Scope

The "nesting" syntax is very(!) confusing.  _function () {

  function makeMysteryFunction(makerValue)
  {
    var newFunction = function doMysteriousThing(param)
    {
      return makerValue + param;
    };
    return newFunction;
  }_

### About Mutability
 - it("should know that variables inside a constructor and constructor args are private", function () ...)

The constructor args ("John Smith") surprised me.  I first guessed "Penny Andrews" was the correct answer.

### Higher Order Functions

line 29 var reduction = _(numbers).reduce(
  function(/* result from last call */ memo, /* current */ x) { return memo + x }, /* initial */ 0);_  
  this style of stuff seems (unnecessarily) confusing.  I just bypass it, as it feels like a million rabbitholes in one.

### About Higher Order Functions
comment: I wish this wasn't so functionally , temptingly simple. It’s really a dumb presentation, cause it’s so easy.  I think what would make a ton more sense is this whole coded .js page and just the pink and black ‘test’ boxes.  The grey text make it MUCH too obvious, and kind of ruins the instructional element - unless the entire idea is only for exposure to these methods.

line 10 -function SwedishChef(age, hobby, mood) {
  Muppet.call(this, age, hobby);
  this.mood = mood;

_this_ is really confusing, inherently but also as a parameter(?!) here?  I am unclear what it references - the age, hobby and mood are in the variables.

_Object.prototype.begetObject = function () {
    function F() {}
    F.prototype = this;
    return new F();
};

newObject = oldObject.begetObject();_

"Beget"?!  REALLY?  Isn't that a Biblical word?!

Starting to not understand at all - perhaps the .prototype method has created a Muppet constructor??  Begat one?!

### What We Have Learnt
line 21  _var i,j,hasMushrooms, productsICanEat = [];_
interesting that the empty array can be called ... that

Jasmine's global _beforeEach_ says the _afterEach_ "resets the variable before continuing."  This would be an interesting tidbit to include in "Testing" lecture.

line 74 _ingredientCount[products[i].ingredients[j]] = (ingredientCount[products[i].ingredients[j]] || 0) + 1;_
No idea what the "or" is doing here


line 84     _chain() together map(), flatten() and reduce()_
  This one ... I don't understand.  Carrie and I worked on it and I understand how she chains them but ... I don't understand the methods.  They are very foreign concepts still.
