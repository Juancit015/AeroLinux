# Changelog

Todos los cambios notables de este proyecto se documentan aquí.

## [Unreleased]

### Added
- Fase 1: Base Debian Trixie + XFCE mínimo ✅
- Dependencias esenciales (fastfetch, wget, nano, codecs, etc.)
- Configuración de live-build (trixie, amd64)
- Lista de paquetes base (ver `aerolinux-fases.txt`)
- README.md y CHANGELOG.md
- aerolinux-fases.txt con roadmap completo
- .gitignore (excluye ISOs, chroots, caché)
- **Fase 2: Tema "Aero" completo** ✅
  - Tema GTK3 creado desde cero (paleta azul/blanco #3C6EB4, #FFFFFF)
  - Menús heredan diseño de Adwaita (diseño compacto, hover azul oscuro)
  - Marcos de ventana xfwm4 con iconos visibles
  - 6 wallpapers oficiales (estilo Fluent) en /usr/share/backgrounds/aero
  - Cursor Bibata-Modern-Ice (blanco, moderno)
  - Iconos elementary por defecto
  - Config base aplicada vía /etc/skel (settings.ini + xsettings.xml + cursor)
  - Tema de ventana: Default (xfwm4)

### Fases Planificadas
- Fase 2: ✅ Completada (Tema GTK3 + xfwm4 + wallpapers + cursor + iconos)
- Fase 3: Instalador Calamares
- Fase 4: Aero Welcome
- Fase 5: AeroStore
- Fase 6: Aero Center
- Fase 7: ISO Beta + pruebas
- Fase 8: Lanzamiento v1.0

## [0.0.1] - Initial Setup
- Estructura del proyecto creada con live-build
- Configuración base de live-build (trixie, amd64)
