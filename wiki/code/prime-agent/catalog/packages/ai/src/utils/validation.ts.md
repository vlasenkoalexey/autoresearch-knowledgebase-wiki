---
title: 'Module: packages/ai/src/utils/validation.ts'
type: catalog
provenance: extracted
module: packages/ai/src/utils/validation.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/utils/`validation.ts`/
symbols:
  coerceWithJsonSchema: coerceWithJsonSchema().
  validateToolArguments: validateToolArguments().
  JsonSchemaObject: JsonSchemaObject#
  applySchemaObjectCoercion: applySchemaObjectCoercion().
  validateToolCall: validateToolCall().
  applySchemaArrayCoercion: applySchemaArrayCoercion().
  coerceWithUnionSchema: coerceWithUnionSchema().
  getValidator: getValidator().
  isValidatorSchema: isValidatorSchema().
  getSubSchemaValidator: getSubSchemaValidator().
  isJsonSchemaObject: isJsonSchemaObject().
  isRecord: isRecord().
  JsonSchemaObject.items: JsonSchemaObject#items.
  hasTypeBoxMetadata: hasTypeBoxMetadata().
  getSchemaTypes: getSchemaTypes().
  JsonSchemaObject.additionalProperties: JsonSchemaObject#additionalProperties.
  JsonSchemaObject.allOf: JsonSchemaObject#allOf.
  JsonSchemaObject.anyOf: JsonSchemaObject#anyOf.
  JsonSchemaObject.oneOf: JsonSchemaObject#oneOf.
  JsonSchemaObject.type: JsonSchemaObject#type.
  JsonSchemaObject.properties: JsonSchemaObject#properties.
  matchesJsonType: matchesJsonType().
  validatorCache: validatorCache.
  TYPEBOX_KIND: TYPEBOX_KIND.
  coercePrimitiveByType: coercePrimitiveByType().
  formatValidationPath: formatValidationPath().
---
# Module: [`packages/ai/src/utils/validation.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts)

## Classes
### `JsonSchemaObject`
- def: [`packages/ai/src/utils/validation.ts:9`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L9)
- signature: `interface JsonSchemaObject`
- members:
  - `additionalProperties` — [`L13`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L13)
  - `allOf` — [`L14`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L14)
  - `anyOf` — [`L15`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L15)
  - `items` — [`L12`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L12)
  - `oneOf` — [`L16`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L16)
  - `properties` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L11)
  - `type` — [`L10`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L10)
- used by: [`coerceWithJsonSchema`](validation.ts.md#coerceWithJsonSchema), [`applySchemaObjectCoercion`](validation.ts.md#applySchemaObjectCoercion), [`applySchemaArrayCoercion`](validation.ts.md#applySchemaArrayCoercion), [`coerceWithUnionSchema`](validation.ts.md#coerceWithUnionSchema), [`getSubSchemaValidator`](validation.ts.md#getSubSchemaValidator), [`isJsonSchemaObject`](validation.ts.md#isJsonSchemaObject), [`getSchemaTypes`](validation.ts.md#getSchemaTypes)

## Functions
- `applySchemaArrayCoercion(value: unknown[], schema: JsonSchemaObject)` — [`L174`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L174)
- `applySchemaObjectCoercion(value: Record<string, unknown>, schema: JsonSchemaObject)` — [`L151`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L151)
- `coercePrimitiveByType(value: unknown, type: string)` — [`L77`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L77)
- `coerceWithJsonSchema(value: unknown, schema: JsonSchemaObject)` — [`L205`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L205)
- `coerceWithUnionSchema(value: unknown, schemas: JsonSchemaObject[])` — [`L193`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L193)
- `formatValidationPath(error: TLocalizedValidationError)` — [`L257`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L257)
- `getSchemaTypes(schema: JsonSchemaObject)` — [`L31`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L31)
- `getSubSchemaValidator(schema: JsonSchemaObject)` — [`L66`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L66)
- `getValidator(schema: TSchema)` — [`L246`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L246)
- `hasTypeBoxMetadata(schema: unknown)` — [`L27`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L27)
- `isJsonSchemaObject(value: unknown)` — [`L23`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L23)
- `isRecord(value: unknown)` — [`L19`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L19)
- `isValidatorSchema(value: unknown)` — [`L62`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L62)
- `matchesJsonType(value: unknown, type: string)` — [`L41`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L41)
- `validateToolArguments(tool: Tool<TSchema>, toolCall: ToolCall)` — [`L292`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L292) — Validates tool call arguments against the tool's TypeBox schema
- `validateToolCall(tools: Tool<TSchema>[], toolCall: ToolCall)` — [`L277`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L277) — Finds a tool by name and validates the tool call arguments against its TypeBox schema

## Module values
- `TYPEBOX_KIND` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L7)
- `validatorCache` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/validation.ts#L6)

