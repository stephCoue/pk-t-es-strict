##  Pas de doublons

<pre>
  <code>
  //  Erreur de syntaxe en mode strict - duplicate arguments
  function faireUnTruc(valeur1, valeur2, valeur1) {
      // code
  }

  //  Erreur de syntaxe en mode strict - duplicate properties
  var object = {
      foo: "bar",
      foo: "baz"
  };
</pre>


Ce sont deux erreurs de syntaxe et elle sont remontées avant même être exécutées.

