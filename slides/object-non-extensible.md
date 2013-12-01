##  Object non-extensible

Une erreur est remontée si l'on tente de modifier un object non-extensible.

<pre><code>
  var testObj = Object.defineProperties({}, {
        prop1: {
            value: 10,
            writable: false // by default
        },
        prop2: {
            get: function () {

            }
        }
  });
  // Echoue en silence en mode non-strict, remonte use erreur en mode strict
  testObj.prop1 = 20;  // Assignation à une propriété en lecture seule
  testObj.prop2 = 30;  // Assignation à une propriété qui n'a une méthode get
</pre>





