# Metodología de Programación Segura: Herramientas para minimizar el riesgo asociado

¿Existen herramientas y/o metodologías que permitan evitar o minimizar el riesgo de que estas
vulnerabilidades asociadas al desarrollo del código se produzcan? La respuesta es afirmativa:

### Analizadores Estáticos

Para evitar este tipo de “bugs” en primer lugar existen analizadores estáticos de código que son capaces de detectar las vulnerabilidades más extendidas. Entre ellos destacamos:
* PMD que funciona para lenguajes como Java, JavaScript, XML, XSL.
* FlawFinder para C.
* LAPSE (OWASP) que funciona como un plugin de Eclipse, y obviamente es para Java.
* Algunas herramientas comerciales son CodeSecure (Armorize), AppScan (IBM), Fortify
(HP). Estas suelen funcionar para diferentes lenguajes (ASP.NET, VB.NET, C#, Java/J2EE,
JSP, EJB, PHP, Classic ASP and VBScript)

### Guías

Por otro lado también existen diferentes guías que recopilan mejores prácticas para el desarrollo de aplicaciones seguras en diferentes lenguajes de programación:
* **ISO Programming languages** – Guide for the Use of the Ada Programming Language in
High Integrity Systems.
* **MISRA:** Guidelines for the use of the C language in critical systems.
* **CERT:** C Secure Coding Standard, Secure Coding in C and C++ y Oracle Secure Coding
Standard for Java.
* **OWASP:*** Secure Coding Practices Quick Reference Guide.
 
### Metodologías completas de programación segura

Por ultimo, cuando se habla de metodologías completas de programación segura, debemos
destacar las siguientes tres:
* The Software Security Framework (SSF).
* OWASP Software Assurance Maturity Model (SAMM).
* Microsoft Security Development Lifecycle (SDL).