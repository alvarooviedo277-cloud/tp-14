USE huertas_abp;


-- Miembros (>=5)
INSERT INTO miembros (nombre, email, telefono, rol, fecha_alta) VALUES
('María Pérez','maria.perez@huerta.org','351-1234567','coordinador','2024-03-01'),
('Juan Gómez','juan.gomez@huerta.org','351-2345678','miembro','2024-04-15'),
('Lucía García','lucia.garcia@huerta.org','351-3456789','miembro','2025-01-10'),
('Roberto Díaz','roberto.diaz@huerta.org','351-4567890','administrador','2023-11-05'),
('Ana Torres','ana.torres@huerta.org','351-5678901','miembro','2025-06-20');


-- Parcelas (>=5)
INSERT INTO parcelas (nombre, ubicacion, area_m2, responsable_id) VALUES
('Parcela A','Sector Norte - Lote 1',30.50,1),
('Parcela B','Sector Norte - Lote 2',25.00,2),
('Parcela C','Sector Sur - Lote 1',40.00,1),
('Parcela D','Sector Sur - Lote 2',18.75,3),
('Parcela E','Invernadero 1',12.00,4);


-- Inventario (>=5)
INSERT INTO inventario (tipo, nombre, cantidad, unidad, descripcion) VALUES
('semilla','Tomate','500','gramos','Semillas de tomate variedad criolla'),
('semilla','Lechuga','300','gramos','Mezcla de lechugas'),
('herramienta','Pala','10','unidad','Pala de mano para trabajar la tierra'),
('herramienta','Rastrillo','4','unidad','Rastrillos medianos'),
('semilla','Zanahoria','400','gramos','Semillas de zanahoria');


-- Cultivos (>=5)
INSERT INTO cultivos (nombre, tiempo_cosecha_dias, descripcion) VALUES
('Tomate',90,'Tomate para consumo fresco y salsa.'),
('Lechuga',45,'Lechuga de hoja para ensaladas.'),
('Zanahoria',75,'Zanahoria de raíz.'),
('Perejil',60,'Hierba aromática.'),
('Zapallo',100,'Variedad de zapallo de estación.');


-- Plantaciones (>=5)
INSERT INTO plantaciones (parcela_id, cultivo_id, sembrado_por, fecha_siembra, cantidad_semillas, estado) VALUES
(1,1,1,'2025-08-01',100,'activa'),
(2,2,2,'2025-09-10',50,'activa'),
(3,3,3,'2025-07-15',200,'activa'),
(4,4,2,'2025-06-01',30,'finalizada'),
(5,5,4,'2025-05-20',20,'fallida');


-- Tareas (>=5)
INSERT INTO tareas (titulo, descripcion, asignada_a, parcela_id, fecha_inicio, fecha_vencimiento, estado, prioridad) VALUES
('Preparar cama de cultivo','Labranza y agregar compost','2',1,'2025-07-28','2025-07-30','completada','alta'),
('Riego semanal parcela A','Riego por goteo y verificación de mangueras','1',1,'2025-08-05','2025-08-12','en_progreso','media'),
('Control de malezas parcela B','Desmalezado ma# tp-14
