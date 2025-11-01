# owl-xmltojs
 Convert OWL(odoo) XML templates to js templates

## Install
npm i -D owl-templates-plugin fast-glob

## Quick start (package.json config)
Add in your app’s package.json:
{
  "owl:templates": ["src/templates/**/*.xml"],
  "owl:templatesOut": "src/templates.js"
}

## vite.config.ts
import { defineConfig } from "vite";
import owlTemplatesPlugin from "owl-templates-plugin";

export default defineConfig({
  plugins: [owlTemplatesPlugin()],
});

## Use in code
import { ui_Counter, ui_Badge } from "./src/templates.js";
// ...
