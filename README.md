# mi_primer_proyecto
Mi primer proyecto 
calificaciones = [85, 67, 92, 74, 58]

print("=== SISTEMA DE CALIFICACIONES ===")
print("Calificaciones iniciales:", calificaciones)

# Acceso mediante indices
print("Primera calificacion:", calificaciones[0])
print("Tercera calificacion:", calificaciones[2])

# Recorrer el vector y clasificar las notas
aprobados = 0
reprobados = 0

for indice, nota in enumerate(calificaciones):
    if nota >= 70:
        print(f"Estudiante {indice + 1}: {nota} - Aprobado")
        aprobados += 1
    else:
        print(f"Estudiante {indice + 1}: {nota} - Reprobado")
        reprobados += 1

# Calculos
promedio = sum(calificaciones) / len(calificaciones)

print("Promedio:", round(promedio, 2))
print("Nota mas alta:", max(calificaciones))
print("Nota mas baja:", min(calificaciones))
print("Aprobados:", aprobados)
print("Reprobados:", reprobados)

# Modificacion de un elemento
calificaciones[1] = 80
print("Vector actualizado:", calificaciones)

nuevo_promedio = sum(calificaciones) / len(calificaciones)
print("Nuevo promedio:", round(nuevo_promedio, 2))

# Busqueda
buscada = 92

if buscada in calificaciones:
    print("La calificacion", buscada, "esta en el vector.")
else:
    print("La calificacion", buscada, "no esta en el vector.")
