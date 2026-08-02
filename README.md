# Aero Linux

Distribución Linux personalizada basada en **Debian Trixie** con escritorio **XFCE**.

## Filosofía

- **Base**: Debian Stable (trixie)
- **Escritorio**: XFCE (ligero, eficiente, personalizable)
- **Paleta**: Azul/blanco estilo Fedora/Anaconda (`#3C6EB4`, `#51A2DA`, `#FFFFFF`, `#F5F5F5`, `#333333`)
- **Objetivo**: Experiencia limpia y moderna enfocada en nuevos usuarios

## Fases de Desarrollo

| Fase | Estado | Descripción |
|---|---|---|
| 1 | En progreso | Base + dependencias esenciales |
| 2 | Pendiente | Tema GTK azul/blanco |
| 3 | Pendiente | Instalador Calamares |
| 4 | Pendiente | Aero Welcome |
| 5 | Pendiente | AeroStore |
| 6 | Pendiente | Aero Center |
| 7 | Pendiente | ISO Beta + pruebas |
| 8 | Pendiente | Lanzamiento v1.0 |

## Dependencias

### Arch Linux
```bash
sudo pacman -S docker git
sudo systemctl enable --now docker
```

### Debian/Ubuntu
```bash
sudo apt update
sudo apt install docker.io git
sudo usermod -aG docker $USER
```

## Construcción

```bash
docker run --rm -it --privileged -v ~/aero-linux:/aero-linux debian:trixie bash
cd /aero-linux
lb config --distribution trixie --archive-areas "main contrib non-free non-free-firmware"
lb build
```

## Contribuir

1. Fork
2. Nueva rama (`feature/nueva-funcionalidad`)
3. Commit (`git commit -m "feat: ..."`)
4. Push y Pull Request

## Licencia

MIT