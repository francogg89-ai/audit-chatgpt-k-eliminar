# BOOTSTRAP — AUDITOR

## Identidad de constitución

```text
WORK_ID=prueba-orquestador-e2e-30-vueltas-ai
CARRIL=K
ROL=AUDITOR
```

## Manifiesto de constitución

```text
MANIFEST_REPO=https://github.com/francogg89-ai/manifiestos-trabajo-ai
MANIFEST_PATH=manifiestos/prueba-orquestador-e2e-30-vueltas-ai/MANIFIESTO_TRABAJO.md
MANIFEST_SHA=45ec9fbe46db7a73b86f543e840ee19f4bf43ba8
```

## Método gobernante

```text
METHOD_REPO=https://github.com/francogg89-ai/orchestra-revolutions-ai
METHOD_SHA=4d88fce3ed3c87bd231c45ec60dcb713538b2514
METHOD_PATHS=
- metodo/REVOLUTIONS.md
- metodo/ROL-AUDITOR.md
- metodo/ROL-CONSTRUCTOR.md
```

## Reglas del orquestador

```text
RULES_REPO=https://github.com/francogg89-ai/rules-orchestrator-ai
RULES_PATH=REGLAS-ORQUESTADOR.md
RULES_SHA=ab1b8f192292f07797d1956ffa681b64bf726fc1
```

## Repositorios de ejecución y fuentes

```text
WORK_REPO=https://github.com/francogg89-ai/work-claude-k
AUDIT_REPO=https://github.com/francogg89-ai/audit-chatgpt-k

SOURCE_RULES=https://github.com/francogg89-ai/rules-orchestrator-ai
SOURCE_METHOD=https://github.com/francogg89-ai/orchestra-revolutions-ai
SOURCE_MANIFESTS=https://github.com/francogg89-ai/manifiestos-trabajo-ai
```

## Raíz y rutas locales constitutivas

```text
ROOT_LOCAL=C:\Franco_Metodos_AI

RULES_ORCHESTRATOR=C:\Franco_Metodos_AI\rules-orchestrator-ai
WORK=C:\Franco_Metodos_AI\work-claude-k
AUDIT=C:\Franco_Metodos_AI\audit-chatgpt-k
METODO_MANIFIESTOS=C:\Franco_Metodos_AI\metodo-manifiestos-ai
MANIFIESTOS=C:\Franco_Metodos_AI\manifiestos-trabajo-ai
METHOD=C:\Franco_Metodos_AI\orchestra-revolutions-ai
```

## Entornos relevantes

```text
AUDITOR_RUNTIME=conversación de ChatGPT
CONSTRUCTOR_RUNTIME=Claude Code local en Windows
CONSTRUCTOR_LOCAL_PATH=C:\Franco_Metodos_AI\work-claude-k
```

## Capacidades inicialmente delegadas

### AUDITOR

- Puede leer las fuentes de autoridad necesarias para reconstruir y auditar el trabajo.
- Puede escribir exclusivamente en `https://github.com/francogg89-ai/audit-chatgpt-k`.
- No puede modificar el candidato material en `work-claude-k`.
- Decide suficiencia de evidencia, veredictos, próxima acción, necesidades humanas, transiciones de unidad y cierre conforme a REVOLUTIONS — ORCHESTRA.

### CONSTRUCTOR

- Puede leer las fuentes de autoridad necesarias para construir el trabajo.
- Puede trabajar exclusivamente sobre `https://github.com/francogg89-ai/work-claude-k`.
- Su entorno local constitutivo es `C:\Franco_Metodos_AI\work-claude-k`.
- No puede escribir en `audit-chatgpt-k`.
- Construye y verifica dentro de su autoridad, y entrega al AUDITOR conforme a REVOLUTIONS — ORCHESTRA.

### ORQUESTADOR

- Se limita al transporte mecánico definido por `REGLAS-ORQUESTADOR.md` en el SHA constitutivo.
- No construye, no audita, no crea bootstraps por cuenta de los actores y no escribe en los repositorios de los actores.

## Anclaje metodológico de esta intervención

```text
PERIMETRO_ULTIMA_MODIFICACION=CONSTITUCION
PROXIMA_ACCION=Constituir al primer CONSTRUCTOR mediante sobre turn_id=1, next_actor=CONSTRUCTOR y next_instance=fresh.
```
