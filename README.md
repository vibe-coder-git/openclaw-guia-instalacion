# 🚀 Cómo instalar OpenClaw en 5 minutos (Ubuntu y macOS)

> Guía rápida para usar OpenClaw en modo Cloud, sin modelos locales ni
> configuraciones complicadas.

------------------------------------------------------------------------

## ✅ Requisitos

-   Ubuntu o macOS\
-   Conexión a internet\
-   Cuenta en OpenAI

❌ No necesitas GPU\
❌ No necesitas 16GB de RAM\
❌ No necesitas Ollama

------------------------------------------------------------------------

## 📦 Paso 1 --- Instalar curl (si no lo tienes)

### Ubuntu

``` bash
sudo apt update && sudo apt install -y curl
```

### macOS (con Homebrew)

``` bash
brew install curl
```

------------------------------------------------------------------------

## ⚡ Paso 2 --- Instalar OpenClaw

``` bash
curl -fsSL https://openclaw.ai/install.sh | bash
```

Verifica la instalación:

``` bash
openclaw --version
```

------------------------------------------------------------------------

## ❗ Si aparece "openclaw: command not found"

En algunos sistemas Linux, la carpeta de instalación puede no estar en
el `PATH`.

Ejecuta:

``` bash
echo 'export PATH="$HOME/.npm-global/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

Luego verifica nuevamente:

``` bash
openclaw --version
```

------------------------------------------------------------------------

## 🔐 Paso 3 --- Login con OpenAI (modo Cloud)

``` bash
openclaw onboard --auth-choice openai-codex
```

Sigue las instrucciones en pantalla para iniciar sesión.

------------------------------------------------------------------------

## 🤖 Paso 4 --- Configurar modelo recomendado

``` bash
openclaw models set openai-codex/gpt-5.3-codex
```

Esto asegura que OpenClaw use el modelo correcto.

------------------------------------------------------------------------

## 📌 Notas importantes

-   Estás usando modelos en la nube.
-   Si tu cuota gratuita se agota, puedes mejorar tu plan en OpenAI.
-   Más adelante puedes crear otra guía sobre cómo usar OpenClaw con
    modelos locales (por ejemplo con Ollama).

------------------------------------------------------------------------

## 🎉 ¡Listo!

Con estos pasos tienes OpenClaw funcionando en menos de 5 minutos.
