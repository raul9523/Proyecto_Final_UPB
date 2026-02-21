# 🏠 HomeFinance: Finanzas Equitativas en Pareja

**HomeFinance** es una aplicación web diseñada para parejas o grupos familiares que buscan una gestión financiera transparente y justa. A diferencia de otras apps de gastos, HomeFinance calcula automáticamente la responsabilidad financiera de cada integrante basándose en su nivel de ingresos, aplicando el principio de proporcionalidad.

---

## 🚀 Características Principales

- **Cálculo Proporcional Automático:** Ingresa los salarios de los aportantes y la app determinará el % de contribución de cada uno.
- **Grupos Familiares:** Crea un grupo e invita a tu pareja o familiares mediante un sistema de invitaciones.
- **Roles de Usuario:** - **Admin:** Gestión de categorías, miembros y configuración del grupo.
  - **Miembro:** Registro de movimientos y visualización de reportes.
- **Gestión de Movimientos:** Registro detallado de ingresos y gastos con categorías personalizadas.
- **Dashboard Dinámico:** Visualización mediante gráficos de torta y barras para entender el comportamiento mensual del gasto.
- **Autenticación Segura:** Acceso mediante Firebase Auth (Correo y Google).

## 🛠️ Tech Stack

Este proyecto utiliza las siguientes tecnologías:

* **Frontend:** [React.js](https://reactjs.org/) (Hooks, Context API).
* **Estilos:** [CSS Modules / Tailwind CSS](https://tailwindcss.com/).
* **Backend & Database:** [Firebase](https://firebase.google.com/) (Cloud Firestore).
* **Autenticación:** Firebase Auth.
* **Gráficos:** [Recharts](https://recharts.org/) o [Chart.js](https://www.chartjs.org/).
* **Control de Versiones:** Git & GitHub.

## 📐 Lógica de Negocio (Distribución de Gastos)

La app utiliza la siguiente fórmula para la repartición equitativa:

$$P_n = \left( \frac{S_n}{\sum S} \right) \times 100$$

*Donde:*
- $P_n$ es el porcentaje de aporte del integrante.
- $S_n$ es el salario individual.
- $\sum S$ es la suma total de salarios del grupo.

*Ejemplo: Si el integrante A gana \$3.000.000 y el integrante B gana \$2.000.000, los gastos se dividirán automáticamente en 60% y 40% respectivamente.*

## 💻 Instalación y Configuración

1. **Clona el repositorio:**
   ```bash
   git clone [https://github.com/tu-usuario/home-finance.git](https://github.com/tu-usuario/home-finance.git)
2. Instala las dependencias:
npm install
3. Configura las variables de entorno:
Crea un archivo .env en la raíz y añade tus credenciales de Firebase:
REACT_APP_FIREBASE_API_KEY=tu_api_key
REACT_APP_FIREBASE_AUTH_DOMAIN=tu_domain
REACT_APP_FIREBASE_PROJECT_ID=tu_project_id
4. Inicia la aplicación:
npm start

📝 Roadmap

[ ] Implementar exportación de reportes en PDF/Excel.

[ ] Notificaciones push para recordatorios de pago de facturas fijas.

[ ] Modo oscuro (Dark Mode).
Desarrollado  por Raúl Serrano - Administrador de Empresas & Desarrollador en Formación.
