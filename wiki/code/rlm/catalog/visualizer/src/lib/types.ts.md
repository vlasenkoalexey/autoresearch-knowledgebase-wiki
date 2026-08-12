---
title: 'Module: visualizer/src/lib/types.ts'
type: catalog
provenance: extracted
module: visualizer/src/lib/types.ts
status: fresh
symbol_base: scip-typescript npm visualizer 0.1.0 src/lib/`types.ts`/
symbols:
  CodeBlock.result: CodeBlock#result.
  RLMIteration: RLMIteration#
  RLMIteration.code_blocks: RLMIteration#code_blocks.
  RLMIteration.prompt.Array.typeLiteral0.content: RLMIteration#prompt.Array:typeLiteral0:content.
  RLMConfigMetadata: RLMConfigMetadata#
  REPLResult.rlm_calls: REPLResult#rlm_calls.
  REPLResult.locals: REPLResult#locals.
  CodeBlock: CodeBlock#
  RLMLogFile.iterations: RLMLogFile#iterations.
  RLMLogFile.metadata: RLMLogFile#metadata.
  RLMLogFile.config: RLMLogFile#config.
  LogMetadata: LogMetadata#
  RLMIteration.final_answer: RLMIteration#final_answer.
  RLMIteration.iteration_time: RLMIteration#iteration_time.
  RLMConfigMetadata.root_model: RLMConfigMetadata#root_model.
  RLMConfigMetadata.max_depth: RLMConfigMetadata#max_depth.
  RLMConfigMetadata.max_iterations: RLMConfigMetadata#max_iterations.
  RLMConfigMetadata.backend: RLMConfigMetadata#backend.
  RLMConfigMetadata.backend_kwargs: RLMConfigMetadata#backend_kwargs.
  RLMConfigMetadata.environment_type: RLMConfigMetadata#environment_type.
  RLMConfigMetadata.environment_kwargs: RLMConfigMetadata#environment_kwargs.
  RLMConfigMetadata.other_backends: RLMConfigMetadata#other_backends.
  RLMLogFile: RLMLogFile#
  extractFinalAnswer: extractFinalAnswer().
  RLMChatCompletion: RLMChatCompletion#
  REPLResult: REPLResult#
  REPLResult.stderr: REPLResult#stderr.
  REPLResult.execution_time: REPLResult#execution_time.
  RLMIteration.prompt: RLMIteration#prompt.
  RLMIteration.prompt.Array.typeLiteral0.role: RLMIteration#prompt.Array:typeLiteral0:role.
  RLMLogFile.fileName: RLMLogFile#fileName.
  RLMLogFile.filePath: RLMLogFile#filePath.
  LogMetadata.totalIterations: LogMetadata#totalIterations.
  LogMetadata.totalCodeBlocks: LogMetadata#totalCodeBlocks.
  LogMetadata.totalSubLMCalls: LogMetadata#totalSubLMCalls.
  LogMetadata.contextQuestion: LogMetadata#contextQuestion.
  LogMetadata.finalAnswer: LogMetadata#finalAnswer.
  LogMetadata.totalExecutionTime: LogMetadata#totalExecutionTime.
  LogMetadata.hasErrors: LogMetadata#hasErrors.
  RLMChatCompletion.prompt: RLMChatCompletion#prompt.
  RLMChatCompletion.response: RLMChatCompletion#response.
  RLMChatCompletion.prompt_tokens: RLMChatCompletion#prompt_tokens.
  RLMChatCompletion.completion_tokens: RLMChatCompletion#completion_tokens.
  RLMChatCompletion.execution_time: RLMChatCompletion#execution_time.
  REPLResult.stdout: REPLResult#stdout.
  CodeBlock.code: CodeBlock#code.
  RLMIteration.type: RLMIteration#type.
  RLMIteration.iteration: RLMIteration#iteration.
  RLMIteration.timestamp: RLMIteration#timestamp.
  RLMIteration.response: RLMIteration#response.
---
# Module: [`visualizer/src/lib/types.ts`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts)

## Classes
### `CodeBlock`
- def: [`visualizer/src/lib/types.ts:19`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L19)
- signature: `interface CodeBlock`
- members:
  - `code` — [`L20`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L20)
  - `result` — [`L21`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L21)
- uses (calls/refs, reference-scoped): [`REPLResult`](types.ts.md#REPLResult)
- used by: [`computeMetadata`](parse-logs.ts.md#computeMetadata), [`extractContextQuestion`](parse-logs.ts.md#extractContextQuestion), [`extractContextVariable`](parse-logs.ts.md#extractContextVariable), [`code_blocks`](types.ts.md#RLMIteration.code_blocks)

### `LogMetadata`
- def: [`visualizer/src/lib/types.ts:55`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L55)
- signature: `interface LogMetadata`
- members:
  - `contextQuestion` — [`L59`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L59)
  - `finalAnswer` — [`L60`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L60)
  - `hasErrors` — [`L62`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L62)
  - `totalCodeBlocks` — [`L57`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L57)
  - `totalExecutionTime` — [`L61`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L61)
  - `totalIterations` — [`L56`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L56)
  - `totalSubLMCalls` — [`L58`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L58)
- used by: [`computeMetadata`](parse-logs.ts.md#computeMetadata), [`parse-logs.ts`](parse-logs.ts.md#scip-typescript-npm-visualizer-0.1.0-src-lib-parse-logs.ts), [`metadata`](types.ts.md#RLMLogFile.metadata)

### `REPLResult`
- def: [`visualizer/src/lib/types.ts:11`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L11)
- signature: `interface REPLResult`
- members:
  - `execution_time` — [`L15`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L15)
  - `locals` — [`L14`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L14)
  - `rlm_calls` — [`L16`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L16)
  - `stderr` — [`L13`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L13)
  - `stdout` — [`L12`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L12)
- uses (calls/refs, reference-scoped): [`RLMChatCompletion`](types.ts.md#RLMChatCompletion)
- used by: [`computeMetadata`](parse-logs.ts.md#computeMetadata), [`extractContextQuestion`](parse-logs.ts.md#extractContextQuestion), [`extractContextVariable`](parse-logs.ts.md#extractContextVariable), [`CodeBlock`](types.ts.md#CodeBlock)

### `RLMChatCompletion`
- def: [`visualizer/src/lib/types.ts:3`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L3)
- signature: `interface RLMChatCompletion`
- members:
  - `completion_tokens` — [`L7`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L7)
  - `execution_time` — [`L8`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L8)
  - `prompt` — [`L4`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L4)
  - `prompt_tokens` — [`L6`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L6)
  - `response` — [`L5`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L5)
- used by: [`rlm_calls`](types.ts.md#REPLResult.rlm_calls)

### `RLMConfigMetadata`
- def: [`visualizer/src/lib/types.ts:36`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L36)
- signature: `interface RLMConfigMetadata`
- members:
  - `backend` — [`L40`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L40)
  - `backend_kwargs` — [`L41`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L41)
  - `environment_kwargs` — [`L43`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L43)
  - `environment_type` — [`L42`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L42)
  - `max_depth` — [`L38`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L38)
  - `max_iterations` — [`L39`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L39)
  - `other_backends` — [`L44`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L44)
  - `root_model` — [`L37`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L37)
- used by: [`parseJSONL`](parse-logs.ts.md#parseJSONL), [`getDefaultConfig`](parse-logs.ts.md#getDefaultConfig), [`parse-logs.ts`](parse-logs.ts.md#scip-typescript-npm-visualizer-0.1.0-src-lib-parse-logs.ts), [`ParsedJSONL`](parse-logs.ts.md#ParsedJSONL), [`config`](types.ts.md#RLMLogFile.config)

### `RLMIteration`
- def: [`visualizer/src/lib/types.ts:24`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L24) — documented in [visualizer-src-lib-types.ts](../../../../concepts/visualizer-src-lib-types.ts.md)
- signature: `interface RLMIteration`
- members:
  - `code_blocks` — [`L30`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L30)
  - `content` — [`L28`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L28)
  - `final_answer` — [`L31`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L31)
  - `iteration` — [`L26`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L26)
  - `iteration_time` — [`L32`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L32)
  - `prompt` — [`L28`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L28)
  - `response` — [`L29`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L29)
  - `role` — [`L28`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L28)
  - `timestamp` — [`L27`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L27)
  - `type` — [`L25`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L25)
- uses (calls/refs, reference-scoped): [`CodeBlock`](types.ts.md#CodeBlock)
- used by: [`computeMetadata`](parse-logs.ts.md#computeMetadata), [`parseJSONL`](parse-logs.ts.md#parseJSONL), [`extractContextQuestion`](parse-logs.ts.md#extractContextQuestion), [`parse-logs.ts`](parse-logs.ts.md#scip-typescript-npm-visualizer-0.1.0-src-lib-parse-logs.ts), [`extractContextVariable`](parse-logs.ts.md#extractContextVariable), [`iterations`](parse-logs.ts.md#ParsedJSONL.iterations), [`iterations`](types.ts.md#RLMLogFile.iterations)

### `RLMLogFile`
- def: [`visualizer/src/lib/types.ts:47`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L47)
- signature: `interface RLMLogFile`
- members:
  - `config` — [`L52`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L52)
  - `fileName` — [`L48`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L48)
  - `filePath` — [`L49`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L49)
  - `iterations` — [`L50`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L50)
  - `metadata` — [`L51`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L51)
- uses (calls/refs, reference-scoped): [`RLMIteration`](types.ts.md#RLMIteration), [`RLMConfigMetadata`](types.ts.md#RLMConfigMetadata), [`LogMetadata`](types.ts.md#LogMetadata)
- used by: [`parseLogFile`](parse-logs.ts.md#parseLogFile), [`parse-logs.ts`](parse-logs.ts.md#scip-typescript-npm-visualizer-0.1.0-src-lib-parse-logs.ts)

## Functions
- `extractFinalAnswer(answer: string | [string, string])` — [`L65`](../../../../../../../raw/code/rlm/visualizer/src/lib/types.ts#L65)

