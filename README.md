# GAME

/*************************************************************
/*
/*        GAME : entorno virtual donde interactuar con el espacio ( BOUNDED ) AGZ ( collision bmp ) sus objetos y /o personajes
/*                los objetos pueden ser interactivos, y tener asociado un hiperenlace ( HTML o tooltip)
/*                los personajes, pueden hablar o proponer juegos. con el sistema quiz & conversacion
/*
*******************************************************************/                                      /\
  /*                                                                                                       / /
 /*                                                                            bound (limites=∞)          / /
 /*       Theather : TV BOX MODEL :                                            bcollide (BMP/0)          / / 
 /*                                                                       AGZ  id.(Escenario≠Scene)     / /
 /*                   ___                                 ___________________________________          / /       /|
 /*         | S(p)   /  /          /       /             /                                  /         / /      / /
 /*         | atm   /  /          /       /             /                                  /         / /      / /
 /*         |      /  /          /       /             /                                  /         / /      / /
 /*         |     /  /          /       /                 p01                            /         / /      / /
 /*         |    /  /          /       /                   x                            /  P(01)  / /      / /           [] > SCREEN - USER
 /*         |   /  /          /       /               p03                              /         /_/      / / 
/*          |  /  /          /       /                 x                              /      |           / /
/*          | /__/          /       /                           p00                  /       |          / /
/*                                                              x                   /        |         / /
 /*          bck           b00     b01              \____________,_____________/             |        | /
/*         \__________________.______________/         people                                !        
 /*                                                    //pre:interactive-sprite.            player0      if1:menu
/*                 cilindric png                       //id.                                dummie     if0:header     
                                                                                                       (si (if) dom) communicate w canvas?
