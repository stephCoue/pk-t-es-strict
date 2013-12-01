
Pour cette raison il est mieux d'utiliser le mode strict dans une fonction.


<pre><code>
  function doSomething() {
    "use strict";
      // En strict mode
  }

  function doSomethingElse() {
      // this doesn't run in strict mode
  }
</pre>