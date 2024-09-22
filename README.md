# APUNTES CONTROL DIGITAL-2do Corte

##METODOS ALGEBRAICOS 
- Metodos que se usan para obtener de terminado comportamiento en un sistema de lazo cerrado
- Su funcion principal es modificar la funcion de transferencia de acuerdo al objetivo deseado
- Existen 2 metodos: por Igualación de modelo y por igualación de coeficientes

## IGUALACIÓN DE MODELO
- La función G(z) es conocida y es de lazo abierto
- se debe Conocer la respuesta deseada representada en una función de transferencia de lazo Cerrado Go(z)

## Ecuaciones
- $$Go(s)=\frac{C(z)G(z)}{1+C(z)G(z)}$$
- $$Go(z)(1+C(z)G(z)= C(z)G(z)$$
- $$Go(z)+ Go(z)C(z)G(z)= C(z)G(z)$$
- $$Go(z)= C(z)G(z)-Go(z)C(z)G(z)$$
- $$Go(z) = C(z)(G(z)- Go(z)G(z)$$
- $$C(z)=\frac{Go(z)}{G(z)-Go(z)G(z)}=\frac{Go(z)}{G(z)(1-Go(z))}$$

*Si G(z) tiene 2 o mas en Z=-1, la retroalimentacio podria no ser implementada, ya que los controladores podrian no ser imnplementables.
