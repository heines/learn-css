<template lang="pug">
  .base-box
    .contents__large
      .c-flexbox
        a.c-btn.p-balloon.p-balloon__top(label="balloon" href="#")
          | text hover show balloon bottom
        a.p-btn-round(href="#")
      .c-flexbox
        a(href="").c-btn.p-btn-middle 上に戻る
        a(href="").c-btn.p-btn-small 上
        a(href="").c-btn.p-btn-triangle 上
        .p-btn-cross-middle__outer
          a(href="").c-btn.p-btn-cross-middle 上に戻る
        a(href="").c-btn.p-btn-bar-middle 上に戻る
      .c-flexbox
        a(href="").c-btn.p-btn-shadow 影付き
        a(href="").c-btn.p-btn-emboss エンボス
        a(href="").c-btn.p-btn-solided 立体
        a(href="").c-btn.p-btn-shutter シャッター
        a(href="").c-btn.p-btn-camera カメラ
        a(href="").c-btn.p-btn-camera-dark カメラ
        a(href="").c-btn.p-btn-camera3 カメラ3
      .c-flexbox
        a.c-btn.p-btn-curtain(href='')
          |カーテン
        a.c-btn.p-btn-light(href='#')
          |光る
        a.c-btn.p-btn-light-white(href='#') 色が逆
      .c-flexbox
        a.c-btn.p-btn-blur(href='' tags='entrance') sky
          .p-btn-blur__bg1
          .p-btn-blur__bg2
        a.c-btn.p-btn-fill-sring(href='#' data-text='testtest')
          span.p-btn-fill-sring__text
            |testtest
      .c-flexbox
        a.c-btn.p-btn-biscuit(href='')
          |オレオ
          br
          |食べたい
        a.c-btn.p-btn-cookie(href='')
          |クッキー
        .p-btn-bite__outer
          a.c-btn.p-btn-bite(href='https://heines.github.io/learn-css/')
            |はらへ
      .c-flexbox
        .p-image-box
          .p-image-box__line
            .p-image-box__img
              img(src='../assets/pakutaso001.jpg')
            p.p-image-box__text Photo by pakutaso
      .c-flexbox
        a.c-btn.p-btn-bgimage(href="https://heines.github.io/learn-css/" texts="pakutaso")
        a.c-btn.p-btn-tag-image(href="https://heines.github.io/learn-css/")
          |擬似要素に画像を追加
        lineShare
      .c-flexbox
        a(href="").c-btn.p-btn-slide-image
        a(href="").c-btn.p-btn-stretch-image
      .c-flexbox
        a(href="").c-btn.p-btn-line-extend
          |線を引く1。文章は長めの方がいいか
        a(href="").c-btn.p-btn-line-extend.p-btn-line-extend--center
          |線を引く2。テストテキスト（modifier 中央から伸びる）
      .c-flexbox
        a(href="").c-btn.p-btn-line-extend.p-btn-line-extend__center
          |線を引く3。テストテキスト（element 中央に線が置かれる）
        a(href="").c-btn.p-btn-line-extend.p-btn-line-extend__center.p-btn-line-extend--center
          |線を引く4。テストテキスト（modifier 中央から伸びる）
      .c-flexbox
        a(href="").c-btn.p-btn-offset
          |テキストがオフセットする。
        a(href="").c-btn.p-btn-offset.p-btn-offset__mark
          |テキストがオフセットする。（マークつき）
      .c-flexbox
        a(href="").c-btn.p-btn-floats
          |テキストが浮かぶ。
        a(href="").c-btn.p-btn-floats.p-btn-floats__line
          |テキストが浮かぶ。（下線つき）
      .c-flexbox
        a(href="").c-btn.p-btn-rolling(text='テキストが前転する')
          |テキストが前転する
      .c-flexbox
        a(href="").c-btn.p-btn-spin
          |回
        a(href="").c-btn.p-btn-spin-string
          .p-btn-spin-string-char0 回
          .p-btn-spin-string-char1 っ
          .p-btn-spin-string-char2 て
          .p-btn-spin-string-char3 出
          .p-btn-spin-string-char4 て
          .p-btn-spin-string-char5 く
          .p-btn-spin-string-char6 る
        a(href="").c-btn.p-btn-fallen-string
          .p-btn-fallen-string-char0 落
          .p-btn-fallen-string-char1 ち
          .p-btn-fallen-string-char2 て
          .p-btn-fallen-string-char3 出
          .p-btn-fallen-string-char4 て
          .p-btn-fallen-string-char5 く
          .p-btn-fallen-string-char6 る
      .c-flexbox
        a(href="").c-btn.p-btn-slidein-string
          p.p-btn-slidein-string__text
            |slide in

      .c-flexbox
        a(href="").c-btn.p-btn-square
          .p-btn-square__line1
          .p-btn-square__line2
          .p-btn-square__line3
          .p-btn-square__line4
          .p-btn-square__text
            |transition
        a(
          href=""
          @mouseover="isOver"
          :class="{'is-over': addIsOver}"
          ).c-btn.p-btn-square
          .p-btn-square__line1
          .p-btn-square__line2
          .p-btn-square__line3
          .p-btn-square__line4
          .p-btn-square__text
            |イベント実装
      .c-flexbox
        a(href="").c-btn.p-btn-lid
          |蓋が開く
        a(href="").c-btn.p-btn-cat-ears
          |猫耳
        .p-btn-bear
          .p-btn-bear__ears-left
          .p-btn-bear__ears-right
          a(href="").c-btn.p-btn-bear__btn
            |くま耳
      .c-flexbox
        a(href="").c-btn.p-btn-ripple
          |波紋
        a(href="").c-btn.p-btn-ripple.p-btn-ripple--fill
          |波紋
        a(href="").c-btn.p-btn-ripple.p-btn-ripple--double
          |波紋
      .c-flexbox
        a(href=''
          @mouseover="isOver"
          @mouseleave="isLeave"
          :class="{'is-leave': addIsLeave}"
          ).c-btn.p-btn-octagram
          |hover
        a(href='').c-btn.p-btn-oct-rotate
          |hover
      .c-flexbox
        a.c-btn.p-btn-brackets(href='')
          .p-btn-brackets__text
            |かっこ
        a.c-btn.p-btn-brackets-jp(href='')
          .p-btn-brackets-jp__open
          .p-btn-brackets-jp__close
          .p-btn-brackets-jp__text
            |かっこ
      .c-flexbox
        a.c-btn.p-btn-gradation(href='')
          |gradation
        a.c-btn.p-btn-radiate(href='')
          |radiate
        a.c-btn.p-btn-float-shadow(href='')
          |shadow
      .c-flexbox
        a.c-btn.p-btn-lighter-round(href='')
          |round light
        a.c-btn.p-btn-lighter-straight(href='')
          |straight light
      .c-flexbox
        a(href='mailto:test@test.com').c-btn.p-btn-mail
          |mail
        button(
          type=submit
          @click="isClicked"
          :class="{'is-clicked': addIsClicked}"
          ).c-btn.p-btn-send
          .p-btn-send__envelope
          .p-btn-send__good
          |send
      .c-flexbox
        a(href='').c-btn.p-btn-light-bulb
          |think
        a(href='').c-btn.p-btn-room-light
          |電気
      .c-flexbox
        a(href='').c-btn.p-btn-capsize
          |ぐるーん
        a(href='').c-btn.p-btn-bar-spin
      .c-flexbox
        a(href='').c-btn.p-btn-reverse
          .p-btn-reverse__front
            |front
          .p-btn-reverse__back
            |back
        a(href='').c-btn.p-btn-flown
          |飛んでった
        a(href='').c-btn.p-btn-flown.p-btn-flown--reverse
          |飛んできた
      .c-flexbox
        a(href='').c-btn.p-btn-fallen
          |落ちる
        a(href='').c-btn.p-btn-snap
          |折れる
        a(href='').c-btn.p-btn-doors
          |開く
      .c-flexbox
        a(href='').c-btn.p-btn-turned-up
          |めくれる
        a(href='').c-btn.p-btn-reopen-book
          .p-btn-reopen-book__front
            |表紙
          .p-btn-reopen-book__default
            |常に見えているページ
          .p-btn-reopen-book__next
            |hoverすると見える
        a(href='').c-btn.p-btn-tile
          |も
          .p-btn-tile__1
          .p-btn-tile__2
          .p-btn-tile__3
          .p-btn-tile__4
      .c-flexbox.c-flexbox--black
        a(href='').c-btn.p-btn-flashing
          |明滅する
        a(href='').c-btn.p-btn-exit
          .p-btn-exit__mark
          .p-btn-exit__outdoors
      .c-flexbox
        .p-btn-list
          .p-btn-list__main
            p.p-btn-list__text
              |select
          .p-btn-list__content1
            |1
          .p-btn-list__content2
            |2
          .p-btn-list__content3
            |3
</template>

<script>
  import lineShare from '../components/lineShare';
  export default {
    name: 'buttons',
    data () {
      return {
        addIsOver: false,
        addIsLeave: false,
        addIsClicked: false
      }
    },
    components: {
      lineShare
    },
    methods: {
      isOver: function(){
        this.addIsOver = true;
        this.addIsLeave = false;
      },
      isLeave: function(){
        this.addIsLeave = true;
      },
      isClicked: function() {
        this.addIsClicked = true;
      }
    }
  }
</script>

<style lang="scss" scoped>
@import '../css/_main.scss';
</style>
