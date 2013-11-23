## L'utilisation de `this`


Un important changement : la valeur `this.prop` de `null` ou `undefined` n’est plus associée à la globale. Mais les valeurs originelles sont conservées.



<pre><code>
  window.color = "black";
  function sayColor() {
      console.log(this.color);
  }

  // Erreur de Typage en mode strict, au lieu de "black"
  sayColor();

  // Erreur de Typage en mode strict, au lieu de "black"
  sayColor.call(null);
</code></pre>

