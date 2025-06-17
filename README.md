# 💻 Examen2 - Cálculo de Pago para Programadores Freelance

Este proyecto en Java permite calcular el **pago total que recibe un programador freelance** en función de varios factores como su experiencia, tipo de contrato, horas trabajadas por cliente y bonos adicionales. El programa también aplica descuentos e impuestos para generar un **reporte final detallado de liquidación**.

---

## 📌 Requisitos

- Java 8 o superior
- IDE (opcional): IntelliJ, Eclipse, VS Code, etc.
- Consola o terminal para entrada/salida

---

## 🧠 ¿Qué hace este programa?

El programa realiza lo siguiente:

1. Solicita información personal del programador (nombre, correo, ciudad, país, etc.).
2. Calcula una tarifa por hora basada en el nivel y los años de experiencia.
3. Solicita datos de 3 clientes, horas trabajadas y bonos adicionales.
4. Calcula el pago bruto por cada cliente.
5. Aplica descuentos (3%) e impuestos (9%).
6. Genera un **reporte detallado de pago** con toda la información ingresada y los cálculos.

---

## 🔢 Fórmulas y lógica usada

- **Tarifa base**: $50/hora
- **Bono por nivel de experiencia**:
  - Junior: $0
  - Senior: $20
- **Bono por experiencia**: `años_experiencia * 1.5`
- **Pago por cliente**: `(horas * tarifa_hora) + bono`
- **Subtotal**: Suma de todos los pagos por cliente
- **Descuento**: 3% del subtotal
- **Impuesto**: 9% del subtotal
- **Total final a recibir**: `subtotal - descuentos - impuestos`

---

## 🏁 ¿Cómo se ve en la terminal?

----- REPORTE DE PAGO -----
Nombre del programador: Ana López
Correo: ana.lopez@example.com
Ciudad: Medellín, Colombia
Fecha de liquidación: 2025-06-17
Tipo de contrato: Freelance
Nivel de experiencia: Senior
Tarifa por hora: $92.5

Detalle por cliente:
Cliente A: $1850.0
Cliente B: $2250.0
Cliente C: $2100.0

Subtotal: $6200.0
Descuentos (3%): $186.0
Impuestos (9%): $558.0
Total a recibir: $5456.0

Formulas usadas 🧠

pagoCliente = (horasTrabajadas * tarifaHoraFinal) + bono

subtotal = suma de pagos por cliente
descuentos = subtotal * 0.03
impuestos = subtotal * 0.09
total = subtotal - descuentos - impuestos

