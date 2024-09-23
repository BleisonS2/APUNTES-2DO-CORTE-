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

💡Ejemplo:


  
### CONCIDERACIONES DE IMPLEMENTACION
- Los compensadores deben ser causales
- El modelo objetivo debe ser estable
-  no deben resultar cancelaciones Polo-Zero
-  $$r <= r$$
-  Los zeros (La fase no minima seran retenidos en lazo cerrado

## IGUALACIÓN DE COEFICIENTES

- Sabiendo que la función G(z) es conocida y es de lazo abierto
- conociendo la ubicación de polos que se desea, a partir de la respuesta deseada, se puede representar en un polinomio caracteríztico
- Es posible obtener la función de trasnsferencia del Controlador C(z) que asegura dicho comportamiento

## LAZO CERRADO
💡Ejemplo:
-Funcion
-Calcular la funcion de transferencia:

$$Go=\frac{k*\frac{0.0043}{z^{2}-1.819z+0.8187}}{1+k*\frac{0.0043}{z^{2}-1.819z+0.8187}}$$

- luego obtendremos:

$$\frac{k * 0.0043}{z^{2}-1.819z+0.8187+k * 0.0043}$$

- Luego igualamos los polinomios (caracteristico en lazo cerrado y caracteristico deseado).

$$z^{2}-1.819+0.8187+k * 0.0043 = z^{2}-1.82+0.881$$

- Ahora comparamos los polinomios.
  
$$z^{2} =z^{2}$$

$$1.819 ≠ 1.82$$

$$k * 0.0043 + 0.8187 = 0.881$$

$$k=14.48$$

No se puede solucionar con acción proporcional.

