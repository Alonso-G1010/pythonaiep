#crear lista para almacenar las ventas de la semana
ventas=[]
#usar un ciclo para ingesar las ventas
for i in range(7): #7 dias de la semana
    venta=float(input(f"ingrese las ventas del dia {i+1}:"))
    ventas.append(venta)

#procesar los datos
total_ventas=sum(ventas)
promedio_ventas=total_ventas/len(ventas)

#condicion para verificar si se alcanzo la meta
meta=5000

if total_ventas>=meta:
    mensaje="felocidades haz alcanzado la meta"
else: 
    mensaje="no se alcanzo la meta"

#imprimir resultado}
print("\n----reorte----")
print(f"total de ventas: $(total_ventas)")
print(f"promedio ${promedio_ventas}")
print(mensaje) 
