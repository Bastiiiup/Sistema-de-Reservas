# Sistema-de-Reservas
- **Estudiante:** Bastian Fuentealba
- **Seccion:** 2
  
# Caso de uso
-- El estudiante puede ver el historial de otras personas
-- Justificacion: el estudiante no deberia poder ver el historial de otras personas solo el adminisitrador

-- Error hay que agregar relacion de <<extend>> desde **Notificar cambio por correo** hacia **Rechazar reserva**
-- Justificacion: nuestro caso nos dice que cada que haya un cambio en la reserva tenemos que notificar al correo

-- Error en la relacion de cancelar reserva y agregar motivo
-- Justificacion: necesitamos poner la relacion <<extend>> entre estos 2 caso de uso ya que agregar motivo es obligatorio por lo que nos dice nuestro caso 

# Diagrama de clases
-- Error reserva no se conecta con sala 
-- Justificacion: estas 2 deberian conectarse ya que no se sabe la informacion con la reserva

-- Error la relacion entre usuario y sala 
-- Justificacion: la relacion de estas 2 tablas no deberia existir ya que usuario se deberia conectar con la tabla reserva

-- Error en la relaciones de gestorNotificaciones con Notificarcorreo y con NotificarSMS
-- Justificacion: estas deberian estar con un adapter o no existir
