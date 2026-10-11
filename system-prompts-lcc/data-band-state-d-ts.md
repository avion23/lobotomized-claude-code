<!--
name: 'Data: band-state.d.ts'
description: >-
  Example hooks-module file (band-state.d.ts) extracted as examples/ with the
  plugin-authoring skill, which points the model at it per ask.
ccVersion: 2.1.296
-->
export type Turn = { seconds: number; tools: number }

declare module 'claude-code' {
  interface PluginState {
    'turn-band': { last: Turn | null; isHidden: boolean }
  }
}
