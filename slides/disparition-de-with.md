##  Disparition de `with`

Il est considéré comme invalide et remonte une erreur de syntaxe dès lors qu'il est parsé.

<pre><code>
  //  Erreur de syntaxe en mode strict
  with (location) {
      console.log(href);
  }

</code></pre>

