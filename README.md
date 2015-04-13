# angular-waffle
The angular-waffle Bower component

The Waffle Generator is a popular method of creating quanta of gibberish that is unnervingly pleasant to read. Use this component to pad out your pages, (or dissertations), where you'd normally use that boring Lorum Ipsum rubbish.

For an example of what it produces, <a href="http://www.mml.co.uk/waffle.php" target="_blank">click here</a>

This is an Angular port of Andrew Clarke's Waffle Generator, written without his permission but hopefully with his consent. I am his nephew after all... it's not like he can't invite me to family functions.

To install the component run:
<pre>
$ bower install angular-waffle
</pre>

You're then given a waffle service that exposes functions.

<pre>
angular
  .module('angularWaffleApp', ['ngWaffle'])
  .controller('ExampleCtrl', function ($scope, $waffle) {

    $scope.title = $waffle.generateTitle();

    $scope.name = $waffle.generateName();

    $scope.waffle1 = $waffle.generateParagraph(2);

    $scope.waffle2 = $waffle.generateParagraph(3);

    $scope.waffle3 = $waffle.generateParagraph(5);

    $scope.waffle4 = $waffle.generateParagraph(1);

    $scope.items = $waffle.generateList(4);

    $scope.quote = $waffle.generateQuote(1);

});
</pre>



<h2>generateTitle()</h2>
<p>Does what it says. It makes a title and stores the name globally for the current instance of Waffle.</p>

<h2>generateName()</h2>
<p>Generates a human name. Surprisingly.</p>

<h2>generateParagraph(num)</h2>
<p>This is the good stuff. Waffle will return [num] lines of gibberish.</p>

<h2>generateList(num)</h2>
<p>If you would like an array of nonsense, specify the quantity of nonsense you would like.</p>

<h2>generateQuote(num)</h2>
<p>The resultant twaddle will be limited to the value you put in as [num]. It will also use the generated title of the page if there is one, and stick an Author's name on the end.</p>

For an example project <a href="https://github.com/Beclamide/angular-waffle-example">Click here</a>

Or, for a demo <a href="http://codepen.io/Beclamide/full/YPBJor">Click here</a>
