# angular-waffle
The angular-waffle Bower component

This is an Angular port of Andrew Clarke's Waffle Generator, written without his permission but hopefully with his consent. I am his nephew after all...

To install the component run:
<pre>
$ bower install angular-waffle
</pre>

You're then given a waffle factory you can use with functions that return biblical quantities of bulls*it.

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

For an example project <a href="https://github.com/Beclamide/angular-waffle-example">Click here</a>