# 🚀 Zphisher Modificado - Soluciones Mejoradas de Tunneling

![Zphisher](https://img.shields.io/badge/Zphisher-Modificado-blue?style=for-the-badge&logo=github)
![Tunneling](https://img.shields.io/badge/Tunneling-Multi_opción-green?style=for-the-badge&logo=cloud)
![Android](https://img.shields.io/badge/Platform-Termux-success?style=for-the-badge&logo=android)

Fork mejorado del popular Zphisher con soluciones robustas de tunneling para demostraciones educativas de phishing ético.

> ⚠️ **NOTA IMPORTANTE**: Este software es estrictamente para fines educativos y de concienciación en seguridad. Úselo solo en entornos controlados con el consentimiento explícito de todos los participantes.

## 📖 Tabla de Contenidos

- [Problemas Resueltos](#-problemas-resueltos)
- [Nuevas Funcionalidades](#-nuevas-funcionalidades)
- [Comparativa de Tunneling](#-comparativa-de-tunneling)
- [Instalación y Configuración](#-instalación-y-configuración)
- [Guía de Uso](#-guía-de-uso)
- [Recomendaciones](#-recomendaciones)
- [FAQ](#-faq)
- [Contribución](#-contribución)

## 🐛 Problemas Resueltos

El script original de Zphisher presentaba fallos críticos con:

### ❌ Problemas con Tunneling Original
- **☁️ Cloudflared**: Servicio poco confiable y conexiones inestables
- **🔗 LocalXpose**: Problemas de conexión y limitaciones de tiempo
- **🌐 Serveo**: Servicio discontinuado en muchas regiones
- **⚡ TryCloudflare**: Bloqueos frecuentes y limitaciones

### ✅ Soluciones Implementadas
- **Soporte nativo para Ngrok** - Túneles estables y confiables
- **Alternativa localhost.run** - Opción sin configuración requerida
- **Modo red local mejorado** - Funcionamiento sin internet
- **Sistema de respaldo automático** - Múltiples opciones de contingencia

## 🛠️ Nuevas Funcionalidades

### 1. ✅ Soporte Nativo para Ngrok
```bash
# Instalación automática de Ngrok
install_ngrok()

# Configuración de authtoken
setup_ngrok_token()

# Inicio de túneles Ngrok
start_ngrok()
```

### 2. ✅ Integración con localhost.run
```bash
# Túneles mediante SSH sin configuración
start_localhostrun()

# Detección automática de URLs
# Sin requisitos de registro
```

### 3. ✅ Modo Red Local Mejorado
```bash
# Cambio de 127.0.0.1 a 0.0.0.0
HOST='0.0.0.0'

# Detección automática de IP local
# Instrucciones claras para conexión WiFi
```

### 4. ✅ Interfaz de Usuario Mejorada
```bash
# Reorganización del menú de túneles
# Mensajes más descriptivos y claros
# Guía visual paso a paso
# Indicadores de estado en tiempo real
```

### 5. ✅ Sistema de Respaldo Automático
```bash
# Múltiples opciones de tunneling
# Fallback automático entre servicios
# Detección de servicios disponibles
```

## 📊 Comparativa de Opciones de Tunneling

| Característica | Ngrok | localhost.run | Red Local | Cloudflared | LocalXpose |
|----------------|-------|---------------|-----------|-------------|------------|
| **Confiabilidad** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐ |
| **Velocidad** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐ | ⭐⭐ |
| **Configuración** | Media | Baja | Baja | Media | Alta |
| **Requiere Internet** | Sí | Sí | No | Sí | Sí |
| **Registro Requerido** | Sí | No | No | No | Sí |
| **Tiempo de Actividad** | Ilimitado | 1 hora | Ilimitado | Variable | Limitado |
| **Recomendado** | **PRIMERA OPCIÓN** | Segunda opción | Sin internet | Emergencia | Último recurso |

## 📥 Instalación y Configuración

### Requisitos Previos
```bash
# Actualizar Termux
pkg update && pkg upgrade

# Instalar dependencias
pkg install git php curl wget -y
```

### Instalación del Script Modificado
```bash
# Clonar el repositorio
git clone https://github.com/tu-usuario/zphisher-modificado.git

# Navegar al directorio
cd zphisher-modificado

# Dar permisos de ejecución
chmod +x zphisher.sh
```

### Configuración de Ngrok (Recomendado)
```bash
# Ejecutar el script
./zphisher.sh

# Seguir las instrucciones para configurar el token
# Obtener token gratuito en: https://dashboard.ngrok.com/auth
```

## 🚀 Guía de Uso

### Opción 1: Ngrok (Recomendada)
```bash
# 1. Registrarse en ngrok.com
# 2. Obtener authtoken gratuito
# 3. Configurar token cuando el script lo solicite
# 4. Disfrutar de túneles estables y confiables
```

### Opción 2: localhost.run (Alternativa)
```bash
# Ventaja: No requiere registro ni configuración
# Desventaja: Puede ser más lento y limitado en tiempo
# Ideal para demostraciones rápidas
```

### Opción 3: Red Local (Sin Internet)
```bash
# Perfecto cuando no hay conexión a internet
# Los participantes deben conectarse a la misma red WiFi
# Acceso mediante la IP local mostrada en pantalla
# Ejemplo: http://192.168.1.5:8080
```

### Opción 4: Cloudflared (Emergencia)
```bash
# Útil cuando otras opciones fallan
# Configuración automática incluida
# Puede presentar inestabilidades
```

### Opción 5: LocalXpose (Último Recurso)
```bash
# Opción de respaldo final
# Requiere configuración manual
# Limitaciones de tiempo y conexión
```

## 🎯 Recomendaciones de Uso

### Para Demostraciones Educativas
1. **✅ Usar Ngrok** como primera opción para máxima confiabilidad
2. **✅ Configurar token previamente** para evitar interrupciones
3. **✅ Probar todas las opciones** antes del taller
4. **✅ Tener plan B** activo (red local como respaldo)

### Optimización de Performance
```bash
# Para mejores resultados:
# - Usar conexión WiFi estable
# - Verificar puertos disponibles
# - Actualizar script regularmente
# - Monitorear estado de túneles
```

### Solución de Problemas Comunes
```bash
# Si Ngrok falla:
./zphisher.sh --option 2  # Cambiar a localhost.run

# Si no hay internet:
./zphisher.sh --option 3  # Usar red local

# Si hay errores de puertos:
./zphisher.sh --port 8081 # Cambiar puerto
```

## ❓ FAQ

### P: ¿Necesito pagar por Ngrok?
**R:** No, Ngrok ofrece un plan gratuito suficiente para demostraciones educativas.

### P: ¿Funciona sin root?
**R:** Sí, todas las opciones funcionan sin root excepto algunas configuraciones avanzadas.

### P: ¿Puedo usar mi propio dominio?
**R:** Sí, Ngrok permite dominios personalizados en planes pagos.

### P: ¿Las capturas se guardan?
**R:** Solo con fines demostrativos y se eliminan después de las sesiones.

### P: ¿Es legal este software?
**R:** Solo para fines educativos con consentimiento de todos los participantes.

## 📈 Beneficios de las Mejoras

### ✅ Mayor Confiabilidad
- Múltiples opciones de tunneling
- Sistema de respaldo automático
- Detección de servicios disponibles

### ✅ Experiencia Mejorada
- Mensajes más claros para participantes
- Interfaz reorganizada e intuitiva
- Guía visual paso a paso

### ✅ Flexibilidad Ampliada
- Funcionamiento con y sin internet
- Soporte para diferentes entornos
- Adaptabilidad a diversas redes

### ✅ Mantenimiento Simplificado
- Actualizaciones automáticas
- Detección de problemas
- Soluciones integradas

## 🤝 Contribución

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

### Áreas de Mejora
- Soporte para más servicios de tunneling
- Mejoras en la interfaz de usuario
- Optimización de performance
- Documentación adicional

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

---

<div align="center">

### ⚠️ **Disclaimer Educativo**
Este software es exclusivamente para fines educativos de concienciación en ciberseguridad. El uso malicioso de estas herramientas es ilegal y no está permitido.

### 🌐 **¿Necesitas Ayuda?**
Abre un [issue](https://github.com/tu-usuario/zphisher-modificado/issues) en GitHub para soporte técnico o preguntas.

</div>

---

**🔄 Mantenimiento**: Este fork se mantiene activamente con actualizaciones regulares y mejoras de seguridad.

**📊 Estadísticas**: Más de 5 opciones de tunneling implementadas con detección automática del mejor servicio disponible.

**🎯 Enfoque**: Educación en seguridad y prevención de ataques de phishing mediante demostraciones controladas.
