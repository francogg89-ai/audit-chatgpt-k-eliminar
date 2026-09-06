# Decisión humana — H2 restauración de continuidad current del CONSTRUCTOR

```text
WORK_ID=prueba-orquestador-e2e-30-vueltas-ai
CARRIL=K
HUMAN_NEED_ID=H2
STOPPED_TURN_ID=22
RELATED_AUDIT_SHA=a511fd1f74fd68eacb769459e1fc6830650d56e3
RELATED_WORK_SHA=72a5bfdd8c5fde8ea61ddc219aaa7943b2184fb7
INSTANCE_REFERENCE_WORK_SHA=89f1249453af4944050fce1e18a51b414245323b
PERIMETRO_ULTIMA_MODIFICACION=CONSTITUCION
VEREDICTO=H2_RESUELTA
PROXIMA_ACCION=Reanudar el loop con el CONSTRUCTOR current restaurado y continuar con la siguiente entrega material de secuencia/ conforme al PLAN aprobado.
```

## Resolución humana literal

```text
Confirmo que la instancia CONSTRUCTOR fresh que produjo WORK_SHA=89f1249453af4944050fce1e18a51b414245323b fue recuperada y quedó nuevamente asociada a current. CONTINUAR
```

## Qué queda resuelto

El HUMANO confirma explícitamente que:

- se recuperó exactamente la instancia CONSTRUCTOR fresh que produjo
  `89f1249453af4944050fce1e18a51b414245323b`;
- esa misma instancia quedó nuevamente asociada a `current`;
- la decisión de control es `CONTINUAR`.

Esto satisface exactamente la necesidad H2 abierta en la auditoría de
`72a5bfdd8c5fde8ea61ddc219aaa7943b2184fb7`.

## Alcance de la resolución

La resolución:

- habilita reanudar esta misma corrida desde los cortes Git vigentes;
- permite que el próximo pase dirigido a CONSTRUCTOR use `next_instance=current`;
- no modifica el manifiesto;
- no modifica el PLAN aprobado;
- no modifica capacidades ni perímetro delegado;
- no reinicia ni desplaza las cadencias periódicas;
- no borra ni reescribe la auditoría de falla de transporte;
- no reclasifica retroactivamente como correcta la entrega producida por la instancia equivocada;
- no autoriza al ORQUESTADOR a sustituir `current` por una instancia distinta en el futuro.

## Continuidad durable

El material de `WORK_SHA=72a5bfdd8c5fde8ea61ddc219aaa7943b2184fb7` ya fue auditado y su contenido material
`1..8` fue comprobado como correcto. No se crea una segunda auditoría para ese mismo
`WORK_SHA`.

La falla de transporte permanece registrada en:

```text
auditorias/72a5bfdd8c5fde8ea61ddc219aaa7943b2184fb7.md
```

La próxima intervención material debe continuar desde ese corte y agregar únicamente el
siguiente elemento esperado conforme al PLAN aprobado.
