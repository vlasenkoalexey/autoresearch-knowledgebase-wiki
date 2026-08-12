---
title: 'Module: packages/ai/src/utils/event-stream.ts'
type: catalog
provenance: extracted
module: packages/ai/src/utils/event-stream.ts
status: fresh
symbol_base: scip-typescript npm @earendil-works/pi-ai 0.7.2 src/utils/`event-stream.ts`/
symbols:
  EventStream.push: EventStream#push().
  EventStream.result: EventStream#result().
  AssistantMessageEventStream: AssistantMessageEventStream#
  EventStream: EventStream#
  EventStream.end: EventStream#end().
  createAssistantMessageEventStream: createAssistantMessageEventStream().
  AssistantMessageEventStream.-constructor: AssistantMessageEventStream#`<constructor>`().
  EventStream.-constructor: EventStream#`<constructor>`().
  EventStream.waiting: EventStream#waiting.
  EventStream.done: EventStream#done.
  EventStream.queue: EventStream#queue.
  EventStream.resolveFinalResult: EventStream#resolveFinalResult.
  EventStream.finalResultPromise: EventStream#finalResultPromise.
---
# Module: [`packages/ai/src/utils/event-stream.ts`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts)

## Classes
### `AssistantMessageEventStream`  ·  implements/extends AsyncIterable, EventStream
- def: [`packages/ai/src/utils/event-stream.ts:68`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L68)
- signature: `class AssistantMessageEventStream`
- members:
  - `<constructor>()` — [`L69`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L69)
- uses (calls/refs, reference-scoped): [`AssistantMessage`](../types.ts.md#AssistantMessage), [`AssistantMessageEvent`](../types.ts.md#AssistantMessageEvent), [`EventStream`](event-stream.ts.md#EventStream)
- used by: [`streamAnthropic`](../providers/anthropic.ts.md#streamAnthropic), [`types.ts`](../../../coding-agent/src/core/extensions/types.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-extensions-types.ts), [`streamOpenAICompletions`](../providers/openai-completions.ts.md#streamOpenAICompletions), [`streamOpenAICodexResponses`](../providers/openai-codex-responses.ts.md#streamOpenAICodexResponses), [`streamBedrock`](../providers/amazon-bedrock.ts.md#streamBedrock), [`streamGoogleVertex`](../providers/google-vertex.ts.md#streamGoogleVertex), [`streamGoogle`](../providers/google.ts.md#streamGoogle), [`streamOpenAIResponses`](../providers/openai-responses.ts.md#streamOpenAIResponses), [`anthropic.ts`](../providers/anthropic.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-anthropic.ts), [`model-registry.ts`](../../../coding-agent/src/core/model-registry.ts.md#scip-typescript-npm-earendil-works-pi-coding-agent-0.7.2-src-core-model-registry.ts), [`streamAzureOpenAIResponses`](../providers/azure-openai-responses.ts.md#streamAzureOpenAIResponses), [`processResponsesStream`](../providers/openai-responses-shared.ts.md#processResponsesStream), [`openai-completions.ts`](../providers/openai-completions.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-openai-completions.ts), [`processWebSocketStream`](../providers/openai-codex-responses.ts.md#processWebSocketStream), [`types.ts`](../types.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-types.ts), [`openai-responses.ts`](../providers/openai-responses.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-openai-responses.ts), [`google.ts`](../providers/google.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-google.ts), [`amazon-bedrock.ts`](../providers/amazon-bedrock.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-amazon-bedrock.ts), [`google-vertex.ts`](../providers/google-vertex.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-google-vertex.ts), [`mistral.ts`](../providers/mistral.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-mistral.ts), [`register-builtins.ts`](../providers/register-builtins.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-register-builtins.ts), [`NODE_OS_SPECIFIER`](../providers/openai-codex-responses.ts.md#NODE_OS_SPECIFIER), [`openai-responses-shared.ts`](../providers/openai-responses-shared.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-openai-responses-shared.ts), [`azure-openai-responses.ts`](../providers/azure-openai-responses.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-azure-openai-responses.ts), [`consumeChatStream`](../providers/mistral.ts.md#consumeChatStream), [`streamMistral`](../providers/mistral.ts.md#streamMistral), [`streamSimple`](../stream.ts.md#streamSimple), [`stream.ts`](../stream.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-stream.ts), [`StreamFunction`](../types.ts.md#StreamFunction), [`stream`](../stream.ts.md#stream), [`streamSimpleAnthropic`](../providers/anthropic.ts.md#streamSimpleAnthropic), [`streamSimpleBedrock`](../providers/amazon-bedrock.ts.md#streamSimpleBedrock), [`streamSimpleGoogle`](../providers/google.ts.md#streamSimpleGoogle), [`faux.ts`](../providers/faux.ts.md#scip-typescript-npm-earendil-works-pi-ai-0.7.2-src-providers-faux.ts), [`streamWithDeltas`](../providers/faux.ts.md#streamWithDeltas), [`EventStream`](event-stream.ts.md#EventStream), [`streamSimpleMistral`](../providers/mistral.ts.md#streamSimpleMistral), [`streamSimpleGoogleVertex`](../providers/google-vertex.ts.md#streamSimpleGoogleVertex), [`streamSimpleOpenAICodexResponses`](../providers/openai-codex-responses.ts.md#streamSimpleOpenAICodexResponses), [`createLazySimpleStream`](../providers/register-builtins.ts.md#createLazySimpleStream)  (+16 more; 7 test-only)

### `EventStream`  ·  implements/extends AsyncIterable
- def: [`packages/ai/src/utils/event-stream.ts:4`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L4)
- signature: `class EventStream`
- members:
  - `<constructor>(isComplete: (event: T) => boolean, extractResult: (event: T) => R)` — [`L11`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L11)
  - `end(method)` — [`L37`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L37)
  - `push(method)` — [`L20`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L20)
  - `result(method)` — [`L63`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L63)
  - `done` — [`L7`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L7)
  - `finalResultPromise` — [`L8`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L8)
  - `queue` — [`L5`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L5)
  - `resolveFinalResult` — [`L9`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L9)
  - `waiting` — [`L6`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L6)
- uses (calls/refs, reference-scoped): [`AssistantMessageEventStream`](event-stream.ts.md#AssistantMessageEventStream), [`ProxyMessageEventStream`](../../../agent/src/proxy.ts.md#ProxyMessageEventStream)  (9 test-only)
- used by: [`streamAnthropic`](../providers/anthropic.ts.md#streamAnthropic), [`registerFauxProvider`](../providers/faux.ts.md#registerFauxProvider), [`streamOpenAICompletions`](../providers/openai-completions.ts.md#streamOpenAICompletions), [`streamOpenAICodexResponses`](../providers/openai-codex-responses.ts.md#streamOpenAICodexResponses), [`streamBedrock`](../providers/amazon-bedrock.ts.md#streamBedrock), [`streamGoogleVertex`](../providers/google-vertex.ts.md#streamGoogleVertex), [`streamGoogle`](../providers/google.ts.md#streamGoogle), [`streamOpenAIResponses`](../providers/openai-responses.ts.md#streamOpenAIResponses), [`streamAzureOpenAIResponses`](../providers/azure-openai-responses.ts.md#streamAzureOpenAIResponses), [`processResponsesStream`](../providers/openai-responses-shared.ts.md#processResponsesStream), [`complete`](../stream.ts.md#complete), [`streamProxy`](../../../agent/src/proxy.ts.md#streamProxy), [`consumeChatStream`](../providers/mistral.ts.md#consumeChatStream), [`streamAssistantResponse`](../../../agent/src/agent-loop.ts.md#streamAssistantResponse), [`AssistantMessageEventStream`](event-stream.ts.md#AssistantMessageEventStream), [`streamMistral`](../providers/mistral.ts.md#streamMistral), [`agentLoop`](../../../agent/src/agent-loop.ts.md#agentLoop), [`streamWithDeltas`](../providers/faux.ts.md#streamWithDeltas), [`agentLoopContinue`](../../../agent/src/agent-loop.ts.md#agentLoopContinue), [`agent-loop.ts`](../../../agent/src/agent-loop.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-agent-loop.ts), [`completeSimple`](../stream.ts.md#completeSimple), [`createLazySimpleStream`](../providers/register-builtins.ts.md#createLazySimpleStream), [`createLazyStream`](../providers/register-builtins.ts.md#createLazyStream), [`handleContentBlockDelta`](../providers/amazon-bedrock.ts.md#handleContentBlockDelta), [`handleContentBlockStop`](../providers/amazon-bedrock.ts.md#handleContentBlockStop), [`proxy.ts`](../../../agent/src/proxy.ts.md#scip-typescript-npm-earendil-works-pi-agent-core-0.7.2-src-proxy.ts), [`handleContentBlockStart`](../providers/amazon-bedrock.ts.md#handleContentBlockStart), [`createAgentStream`](../../../agent/src/agent-loop.ts.md#createAgentStream), [`endAgentStreamOnError`](../../../agent/src/agent-loop.ts.md#endAgentStreamOnError), [`forwardStream`](../providers/register-builtins.ts.md#forwardStream), [`ProxyMessageEventStream`](../../../agent/src/proxy.ts.md#ProxyMessageEventStream), [`startWebSocketOutputOnFirstEvent`](../providers/openai-codex-responses.ts.md#startWebSocketOutputOnFirstEvent)  (41 test-only)

## Functions
- `createAssistantMessageEventStream()` — [`L85`](../../../../../../../../raw/code/prime-agent/packages/ai/src/utils/event-stream.ts#L85) — Factory function for AssistantMessageEventStream (for use in extensions)

