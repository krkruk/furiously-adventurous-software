================================================================================
SOLID
================================================================================

Wstęp
--------------------------------------------------------------------------------

Oprogramowanie zorientowane obiektowo (OOP) bywa trudne w tworzeniu
i utrzymywaniu. Wprowadzone abstrakcje dość często nie są w stanie sprostać
ewolucji kodu i jego rozszerzania. Z pomocą przychodzi 5 podstawowych zadań
umożliwiające okiełznać potęgę OOP i wykorzystać ją do stworzenia
rozszerzalnego kodu.

Stosując reguły zasady SOLID należy mieć również na względzie, iż nie są
one lekarstwem na wszystko. Kurczowe trzymanie się tych reguł może być
równie, o ile nie bardziej, szkodliwe niż ich brak. Należy zachować umiar
i pamiętać, że musi istnieć istotny powód do modyfikacji kodu.

Single Responsibility Principle
--------------------------------------------------------------------------------

**Single Responsibility Principle** (SRP) - reguła pojedynczej 
odpowiedzialności definiuje się ją następująco

    "Obiekt powinien mieć tylko jeden powód do zmiany"
    -- za źródłem [#martinAgile]_.

Zgodnie z regułą, dany moduł, klasa lub funkcja powinna mieć tylko jedną
odpowiedzialność (funkcjonalność), którą wykonuje. Co to jednak oznacza?

W świecie ludzi ponoć normalnych, regułę SRP można zwizualizować za pomocą
maszyny stanu - pralki. Oczywiste jest, że pralka pierze. Pranie odbywa się
według określonego programu przechodząc jego poszczególne etapy (stany).
Generalnie, odpowiedzialnością pralki jest pranie. Zdaje się, że byłoby
niedorzecznością wyposażyć pralkę w dodatkową funkcję: odkurzanie.

W świecie oprogramowania podobne sytuacje występują, choć przeważnie w subtelny
sposób. Załóżmy istnienie klasy:

.. graphviz::
   :alt: Diagram klas
   :caption: Diagram klas
   :align: center

   digraph ClassDiagram {
       node[shape=record]
       MATH_CLASS[label = "{SophisticatedComputation|+compute() : int[]}"];

       MATH_CLASS;
   }

Open-Closed Principle
--------------------------------------------------------------------------------

Liskov Substitution Principle
--------------------------------------------------------------------------------

Interface Segregation
--------------------------------------------------------------------------------

Dependency Inversion Principle
--------------------------------------------------------------------------------

.. rubric:: Przypisy

.. [#martinAgile] Martin Robert C., *Zwinne wytwarzanie oprogramowania. Najlepsze zasady, wzorce i praktyki*, Helion, 2015
