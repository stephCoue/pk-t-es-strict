
Donc une valeur doit être assignée à `this.prop` sinon elle reste `undefined`. Cas conséquent : l'appel d'un Constructeur sans le `new` est aussi affecté.

<pre><code>
  function Person(name) {
      this.name = name;
  }

  // Error in strict mode
  var me = Person("Steph");

  </pre>

Dans ce code `this` est `undefined` quand on appelle la fonction Constructeur Person() sans `new`. En mode non-strict `this` sera remplacé par la variable globale et `name` assigné à la propriété de la globale.

