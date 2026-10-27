<!--
name: 'Data: pane-state.d.ts'
description: >-
  Example hooks-module file (pane-state.d.ts) extracted as examples/ with the
  plugin-authoring skill, which points the model at it per ask.
ccVersion: 2.1.310
-->
export type ToolCall = { id: string; tool: string; isDone: boolean }

declare module 'claude-code' {
  interface PluginState {
    'tool-calls': { calls: Shaped<ToolCall[]> }
  }
}
