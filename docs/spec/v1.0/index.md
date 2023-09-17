---
title: SLSA仕様
description: SLSA は、サプライ チェーンのセキュリティを記述し、段階的に改善するための仕様であり、業界の合意によって確立されています。これは、セキュリティ保証の強化を説明する一連のレベルに編成されています。これは SLSA 仕様の**version 1.0** であり、SLSA レベルを定義します。
---

SLSA は、サプライ チェーンのセキュリティを記述し、段階的に改善するための仕様であり、業界の合意によって確立されています。これは、セキュリティ保証の強化を説明する一連のレベルに編成されています。

これは SLSA 仕様の**version 1.0** であり、SLSA レベルと、出所を含む推奨される認証形式を定義しています。

{%- for section in site.data.nav.v10 %}
{%- if section.children %}

## {{ section.title }}

{{ section.description }}

| Page | Description |
| ---- | ----------- |
{%- for child in section.children %}
| [{{child.title}}]({{child.url | relative_url}}) | {{child.description}} |
{%- endfor %}

{%- endif %}
{%- endfor %}
