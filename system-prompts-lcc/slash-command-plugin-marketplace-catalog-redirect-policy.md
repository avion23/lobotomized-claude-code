<!--
name: '/plugin marketplace: catalog redirect policy'
description: >-
  Middle fragment of the marketplace-catalog redirect refusal stating the
  cross-origin redirect rules (https, no loopback/link-local/metadata hosts).
ccVersion: 2.1.296
-->
a server-chosen cross-origin redirect must use https:// and must not point at a loopback, link-local, or cloud-metadata host (only a hop that stays on the origin you started from is exempt): 
