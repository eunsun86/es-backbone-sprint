# Siskel

Siskel은 간단한 영화 평가를 할 수 있는 웹입니다. 우리는 이 어플리케이션을 사용하여 Backbone.js 이벤트가 어떻게 구동되는지와 MVC에 대해서 탐구할 것입니다.

## Environment

### Requirements

  - Bower

### Installing Dependencies

```bash
bower install
```

## 목표

Siskel은 사용자가 영화를 '라이크' 또는 '안(?) 라이크'를 할 수 있고 다양한 종목(제목, 연도, 등급 및 사용자가 좋아하는 상태)별로 영화 목록을 정렬도 할 수 있습니다. 현재 코드 베이스는 필요한 기능 요소 대부분을 가지고 있지만 정렬하고 '라이크'를 할 수 있는 모든 기능이 빠져 있습니다. 이 프로젝트의 목표는 module을 연결하여 올바르게 작동하도록 기능을 구현하는 것입니다.

## 내용
이 프로젝트의 핵심은 Backbone.js 이벤트 시스템을 이해하는 것입니다. 이 문서는 Backbone.js에서 이미 만들어 놓은 굉장히 많은 이벤트 목록을 제공합니다. 이 프로젝트에서 가장 중요한 두 가지는 `change` 이벤트와 `sort` 이벤트 입니다.

[Backbone Events](http://backbonejs.org/#Events-catalog)

Backbone.js는 [`comparator`](http://backbonejs.org/#Collection-comparator) 속성이 지정되면 collection을 자동으로 해당 속성 기준으로 정렬시켜 줍니다. [`comparator`](http://backbonejs.org/#Collection-comparator) 속성의 값은 `string`이나 `function`이 될 수 있습니다.

collection이 자체적으로 자동 정렬을 할수 있지만, 때로는 수동으로 다시 정렬해야하는 경우가 있습니다. 필요시 [`sort()`](http://backbonejs.org/#Collection-sort)를 이용하여 수동으로 정렬을 수행할 수 있습니다. 단 여러분이 `comparator`를 지정 해놨다는 가정하에 작동됩니다.

## 기본 TODO

test를 통과하게 만들어 주세요.

- test는 여러분이 app에서 module들을 올바른 연결을 유도하도록 만들어 졌습니다. 각 테스트의 목표가 무엇인지 이해하기 위해 test source code를 읽으세요.

## 고급 TODO

- 양방향으로 정렬(sorting)이 되도록 만드세요. 라디오 버튼을 처음 클릭하면 한 방향으로 정렬되고 동일한 버튼을 다시 클릭하면 반대 방향으로 정렬 되도록 하세요.
