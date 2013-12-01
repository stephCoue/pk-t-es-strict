##  eval()

ECMAScript apporte un lot de changements à `eval()`; le plus significatif est que les variables ou fonctions declarées dans eval() ne sont plus créées dans le “scope container”



<pre><code>
  (function() {

    eval("var x = 10;");

    // En mode non-strict , log 10
    // Erreur de reférence en mode strict
    console.log(x);

  }());

</pre>

Toute variable ou fonction crée dans `eval()` <strong>reste</strong> dans `eval()`. Après, rien n'empêche d'assigner la valeur retour de `eval()`…



