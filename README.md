# diagram gallery

## [plantuml](https://github.com/plantuml/plantuml)

as its name, it is good at drawing all UML diagram.

### setup tool

please refer to [here](https://plantuml.com/faq-install)

- install

  - Java
  - Graphviz (Graphviz dot) -- **this is an optional** because New Java-based diagram generation engine "Smetana"

    ```
    brew install graphviz
    ```

  - download plantuml.jar

    to use New Java-based diagram generation engine "Smetana", need to include this in .puml file

    ```
    !pragma layout smetana
    ```

- command line

  ```shell
  # testing dot
  java -jar plantuml.jar -testdot

  # testing graph generation
  java -jar plantuml-1.2022.7.jar  /Volumes/dao/workspace/anti-bot/docs/api-gateway.puml
  ```

there are a lot of enhancement to make productivity, such as

- visualising software architecture [C4-Model](https://github.com/plantuml-stdlib/C4-PlantUML)
- [WBS](./plantuml/wbs.puml)
- [YAML](./plantuml/yaml.puml)
- [JSON](./plantuml/json.puml)

### themes

- [themes](https://github.com/plantuml/plantuml/tree/master/themes)
- [themes-gallery](https://bschwarz.github.io/puml-themes/gallery.html)

there are 2 directives `theme` or `include` working for theme

```
!theme <theme_name>
!theme foo from /path/to/themes/folder
!theme amiga from https://raw.githubusercontent.com/plantuml/plantuml/master/themes

'or
!include <url>
```

### further readings

- [guide](https://plantuml.com/)
- [live editor](https://www.plantuml.com/plantuml/uml/)

## [mermaid](https://github.com/mermaid-js/mermaid)

most like plantuml, it is a good and easy tool to draw `sequence diagram`, `entity relationship diagram`, `class diagram`, `state diagram` and `gitgraph diagram`.

`mermaid ./mermaid/git-graph.mmd`

[c4-model example](https://mermaid.live/view#pako:eNqdVm1r2zAQ_iuHyYcU0i59-1K2Qd5aCit0TQsbGIpsnxNRWwqSvDaU_vfJkpXIjrJ29Rdb5zs99-genfQapTzD6CIC_UzOJpwpfFExA_MoqgqE-VoqLKH5BxklC0FKyLmAa20SDBWMCXuibNH4uvhZ_XslqMTHMa9YRsS6nwwHEEe1vzMN4-gAXl0MwC0KyVk_raTiJYqR86_nnzRGGMVRbR-BcwOeg1oiJNpzAM9ULWFlJiKFsQFJUw2o5JGG2ws2DoKN6wzN0w18nL2oTfAkGDyxmWYo0800brK9eUyDU03_TfprIr58f5_6FtRWq29fI7PQ-ypqgYuCP8sNugTF4Q_FZ6BMq6EkinIGJOGVqrOioo0-AMIyKMkTwoqsS2wSaq9DUDLHXcl0FOOVxZGaJqY0djCr42-IzlILF4PU5ooLlECKwq1pqg2GQO26S3CzCAOPoBKESZLWbnqEKj3ylLObpEfxpEvxxHBsU-tWzBdJs0tHzYruDRoHgsZOV9KOP7yVgNUdoaAMjzxt--hvYeLb2phNMzssCS0aeJvMvU6AGjFq1BuaCi55rmD2ki4JWyCgH2LQQyJoQKYB0lOYEkUSIvGz7C2oD7ut52m3nqcWJfEVHC7UzworbBK_DCR-CcZjf9b7atEC8EpwFQC5eg_kI0vjyWA72HxuPtx7TO-w8Pu-35geJEqvc1vfrYO30TueIT8jujmyTDY6kk0XuLm_DYbqgNZ51IrVbbDVWB9WGVE4K7DucXO1LtAn1cv1QTrhBRff4khgViP3koWzLASurYmLTJ8pvuNBG0GntzP7lmmvPq1deFLYWvbqvbpj5HkuUf3SpvP9IIG1_m-I39p0eDz8OMjksyBnww6zw_N3YdtFbuG6OvmwztbBaOVx4oO2wX-QtT5H9K0qp4t-Lz2bL8kKr9kdf9Zxpltoo-sezn6sp4sGkc5QKy_T9zZzCsaR3pWlXoMLc9HISVWoOIrZm3atrBgzqg-46EKJCgcRqRSfr1nqxtZnai921vj2F-uvN3c)

### further readings

- [guide](https://mermaid-js.github.io/mermaid/)
- [live editor](https://mermaid.live/)

## [Diagram as Code](https://diagrams.mingrammer.com/)

a good tool to draw architecture diagram for cloud-based system.

- [guide](https://diagrams.mingrammer.com/docs/guides/diagram)

## online drawing

- [ProcessOn](https://www.processon.io/)
- [draw.io / diagrams.net](https://app.diagrams.net/)

## whiteboard

- handwritten [whiteboard](https://excalidraw.com/)
- [auto draw](https://www.autodraw.com/)

## extensions for vs code

- [PlantUML](https://marketplace.visualstudio.com/items?itemName=jebbs.plantuml)
- [Markmap](https://marketplace.visualstudio.com/items?itemName=gera2ld.markmap-vscode)
- Mermaid diagram support to VS Code's **builtin markdown preview**

## others

- [colourful & text sequence diagram](http://echoma.github.io/text_sequence_diagram/)
- [js-sequence-diagrams](https://bramp.github.io/js-sequence-diagrams/)
- [flowchart](https://github.com/adrai/flowchart.js)
- [diagrams for engineers](http://go.drawthe.net/)
- [Diagrams as code 2.0](https://structurizr.com/)
- [Creates diagrams from textual descriptions!](https://kroki.io/)
- [Text to UML](https://modeling-languages.com/text-uml-tools-complete-list/)

## further readings

### [C4 Model](https://c4model.com/#Abstractions)

The C4 model considers the static structures of a software system in terms of containers, components and code.

A software system is made up of one or more containers (web applications, mobile apps, desktop applications, databases, file systems, etc), each of which contains one or more components, which in turn are implemented by one or more code elements (e.g. classes, interfaces, objects, functions, etc).

Visualising this hierarchy of abstractions is then done by creating a collection of Context, Container, Component and (optionally) Code (e.g. UML class) diagrams. This is where the C4 model gets its name from.

Different levels of zoom allow you to tell different stories to different audiences.

1. Level 1: System Context diagram
2. Level 2: Container diagram
3. Level 3: Component diagram
4. Level 4: Code
