# Atividade Three.js — Cena 3D Interativa

Atividade prática da disciplina de Interface Humano-Computador utilizando **Three.js** para renderização de um modelo 3D obtido do Sketchfab.

## Modelo utilizado

**Constable's House** — por ProjectEternal  
Link de origem: https://sketchfab.com/3d-models/constables-house-f5f9ab348b4540efac04885ac6a8a1c5  
Licença: CC Attribution

## Como executar

> **Importante:** o arquivo `scene.gltf` precisa ser servido por um servidor HTTP local (não funciona abrindo direto pelo sistema de arquivos).

### Opção 1 — VS Code + Live Server

Instale a extensão **Live Server** no VS Code, clique com o botão direito no `index.html` e escolha *"Open with Live Server"*.

### Opção 2 — Python (já vem instalado na maioria dos sistemas)

```bash
python -m http.server 8080
```

Depois acesse `http://localhost:8080` no navegador.

## Funcionalidades implementadas

- Modelo 3D carregado via `GLTFLoader`
- `OrbitControls` com rotação, zoom e pan
- Luz ambiente + luz direcional com sombras
- Loop de animação com `requestAnimationFrame`
- Resize handler para câmera e renderer

## Tecnologias

- [Three.js](https://threejs.org/) v0.176.0 (via CDN)
- HTML5 / JavaScript (ES Modules)
