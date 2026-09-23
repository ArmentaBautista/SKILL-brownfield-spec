# Brownfield Spec-Driven Development Skill

Este repositorio incluye un skill especializado para automatizar el levantamiento de especificaciones iniciales (**Core SPEC**) en proyectos *brownfield*, documentando la realidad técnica, la deuda acumulada y generando diagramas en Mermaid.

---

## 📂 Dónde colocar el archivo del Skill por Herramienta

Para que tus agentes detecten y ejecuten este skill de forma nativa, coloca el archivo `brownfield-spec.md` en las siguientes rutas (según la herramienta que utilices):

### 1. Antigravity (Desktop / CLI / Extensión VS Code)
Colócalo dentro del workspace local como un skill de agente:
* **Ruta en el proyecto:** `.agents/skills/brownfield-spec/SKILL.md`
* *(Opcional Global)*: `~/.gemini/antigravity-cli/skills/brownfield-spec/SKILL.md`

### 2. OpenCode (Desktop / CLI)
OpenCode lee los agentes personalizados desde el directorio de configuración local:
* **Ruta en el proyecto:** `.opencode/agent/brownfield-spec.md`
* *(Invocación)*: Usa el comando `--agent brownfield-spec` en CLI o cámbialo desde la interfaz de OpenCode con `/agent brownfield-spec`.

### 3. Kilo Code (CLI / Extensión VS Code)
Kilo Code interpreta las reglas de comportamiento directamente en su carpeta dedicada:
* **Ruta en el proyecto:** `.kilo/rules/brownfield-spec.md`
* *(Opcional en `kilo.jsonc`)*: Asegúrate de registrarlo en la raíz del proyecto agregándolo a tu archivo de configuración:
  ```json
  {
    "instructions": [
      ".kilo/rules/brownfield-spec.md"
    ]
  }

### 4. Codex
Codex utiliza directorios de instrucciones específicas para el contexto del proyecto:
* **Ruta en el proyecto:** .codex/rules/brownfield-spec.md

### 5. Claude Code (CLI)
Claude Code busca instrucciones personalizadas o comandos del sistema en el directorio local:
* **Ruta en el proyecto:** .claude/commands/brownfield-spec.md
* **(Alternativa Global):** ~/.claude/commands/brownfield-spec.md

### 6. 🚀 Ejemplos de Uso
A continuación se muestran un par de ejemplos prácticos de cómo invocar e interactuar con el skill una vez que lo tienes configurado en tu entorno:

**Ejemplo 1:** Iniciando la Fase 1 en OpenCode CLI
Al iniciar una sesión apuntando al agente, este se encargará de saludarte y guiarte con la estructura inicial:

  ```
opencode --agent brownfield-spec

  
