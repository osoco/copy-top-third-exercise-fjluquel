copyTopThird: aPicture
|tempHeight|
//Obtenemos el alto de aPicture
tempHeight := aPicture height.
//Copiamos filas desde 1 hasta hasta el primer tercio a partir del segundo tercio de la altura
1 to: (tempHeight/3) do: [:i | aPicture copyRow: i toRow: 2*tempHeight/3+i].
^aPicture
