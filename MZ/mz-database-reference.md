# RPGツクールMZのデータベース参照表

## アクター

| カラム名     | 名称           |
| ----         | ----           |
|id            |ID              |
|battlerName   |戦闘グラフィック|
|characterIndex|歩行インデックス|
|characterName |歩行グラフィック|
|classId       |職業ID          |
|equips        |初期装備        |
|faceIndex     |顔インデックス  |
|faceName      |顔グラフィック  |
|traits        |特徴            |
|initialLevel  |初期レベル      |
|maxLevel      |最大レベル      |
|name          |名前            |
|nickname      |二つ名          |
|note          |メモ            |
|profile       |プロフィール    |

## 職業

| カラム名     | 名称           |
| ----         | ----           |
|id            |ID              |
|expParams     |経験値曲線(0:基本値	1:補正値	2:増加度A	3:増加度B)|
|traits        |特徴            |
|learnings     |習得スキル      |
|name          |名前            |
|note          |メモ            |
|params        |能力値曲線      |

## スキル

| カラム名       | 名称           |
| ----           | ----           |
|id              |ID              |
|animationId     |アニメーションID|
|damage          |ダメージ        |
|description     |説明            |
|effects         |使用効果        |
|hitType         |命中タイプ      |
|iconIndex       |アイコンIndex   |
|message1        |メッセージ1     |
|message2        |メッセージ2     |
|mpCost          |消費MP          |
|name            |名前            |
|note            |メモ            |
|occasion        |使用可能時      |
|repeats         |連続回数        |
|requiredWtypeId1|必要武器タイプ1 |
|requiredWtypeId2|必要武器タイプ2 |
|scope           |効果範囲        |
|speed           |速度補正        |
|stypeId         |スキルタイプID  |
|successRate     |成功率          |
|tpCost          |消費TP          |
|tpGain          |得TP            |
|messageType     |メッセージタイプ|

## アイテム

| カラム名       | 名称           |
| ----           | ----           |
|id              |ID              |
|animationId     |アニメーションID|
|consumable      |消耗            |
|damage          |ダメージ        |
|description     |説明            |
|effects         |使用効果        |
|hitType         |命中タイプ      |
|iconIndex       |アイコンIndex   |
|itypeId         |アイテムタイプID|
|name            |名前            |
|note            |メモ            |
|occasion        |使用可能時      |
|price           |価格            |
|repeats         |連続回数        |
|scope           |効果範囲        |
|speed           |速度補正        |
|successRate     |成功率          |
|tpGain          |得TP            |

## 武器

| カラム名       | 名称           |
| ----           | ----           |
|id              |ID              |
|animationId     |アニメーションID|
|description     |説明            |
|etypeId         |装備タイプID    |
|traits          |特徴            |
|iconIndex       |アイコンIndex   |
|name            |名前            |
|note            |メモ            |
|params          |能力値          |
|price           |価格            |
|wtypeId         |武器タイプID    |

## 防具

| カラム名       | 名称           |
| ----           | ----           |
|id              |ID              |
|atypeId         |防具タイプID    |
|description     |説明            |
|etypeId         |装備タイプID    |
|traits          |特徴            |
|iconIndex       |アイコンIndex   |
|name            |名前            |
|note            |メモ            |
|params          |能力値          |
|price           |価格            |

## 敵キャラ

| カラム名       | 名称           |
| ----           | ----           |
|id              |ID              |
|actions         |行動パターン    |
|battlerHue      |色相            |
|battlerName     |戦闘グラフィック|
|dropItems       |ドロップアイテム|
|exp             |経験値          |
|traits          |特徴            |
|gold            |所持金          |
|name            |名前            |
|note            |メモ            |
|params          |能力値          |

## 敵グループ

| カラム名       | 名称           |
| ----           | ----           |
|id              |ID              |
|members         |グループ        |
|name            |名前            |
|pages           |バトルイベント  |
|note            |メモ            |

## ステート

| カラム名          | 名称           |
| ----              | ----           |
|id                 |ID              |
|autoRemovalTiming  |自動解除のタイミング|
|chanceByDamage     |確率(ダメージで解除)|
|iconIndex          |アイコンIndex   |
|maxTurns           |継続ターン数(最長)|
|message1           |メッセージ1(アクターがこの状態になったとき)|
|message2           |メッセージ2(敵キャラがこの状態になったとき)|
|message3           |メッセージ3(この状態が継続しているとき)|
|message4           |メッセージ4(この状態が解除されたとき)|
|minTurns           |継続ターン数(最短)|
|motion             |モーション|
|name               |名前            |
|note               |メモ            |
|overlay            |重ね合わせ|
|priority           |優先度|
|releaseByDamage    |ダメージで解除|
|removeAtBattleEnd  |戦闘終了時に解除|
|removeByDamage     |確率(ダメージで解除)|
|removeByRestriction|行動制約によって解除|
|removeByWalking    |歩数で解除|
|restriction        |行動制約|
|stepsToRemove      |歩数(歩数で解除)|
|traits             |特徴            |
|messageType        |メッセージタイプ|

## アニメーション

| カラム名        | 名称           |
| ----            | ----           |
|id               |ID              |
|displayType      |表示タイプ      |
|effectName       |ファイル名      |
|flashTimings     |フラッシュ      |
|name             |名前            |
|offsetX          |オフセットX     |
|offsetY          |オフセットY     |
|rotation         |回転            |
|scale            |拡大率          |
|soundTimings     |効果音          |
|speed            |速度            |

## タイルセット

| カラム名        | 名称           |
| ----            | ----           |
|id               |ID              |
|flags            |通行            |
|mode             |モード          |
|name             |名前            |
|note             |メモ            |
|tilesetNames     |画像            |

## コモンイベント

| カラム名        | 名称           |
| ----            | ----           |
|id               |ID              |
|list             |実行内容        |
|name             |名前            |
|switchId         |スイッチ        |
|trigger          |トリガー        |

## システム

| カラム名         | 名称           |
| ----             | ----           |
|advanced          |高度な設定      |
|airship           |飛行船          |
|armorTypes        |防具タイプ      |
|attackMotions     |攻撃モーション  |
|battleBgm         |音楽(戦闘BGM)   |
|battleback1Name   |アニメーション・戦闘テスト(背景1)|
|battleback2Name   |アニメーション・戦闘テスト(背景2)|
|battlerHue        |アニメーション・戦闘テスト(色相)|
|battlerName       |アニメーション・戦闘テスト(戦闘グラフィック)|
|battleSystem      |戦闘システム|
|boat              |小型船|
|currencyUnit      |通貨単位|
|defeatMe          |音楽(敗北ME)|
|editMapId         |最後に編集したマップID|
|elements          |属性|
|equipTypes        |装備タイプ|
|gameTitle         |ゲームタイトル|
|gameoverMe        |音楽(ゲームオーバーME)|
|itemCategories    |アイテムカテゴリー|
|locale            |言語|
|magicSkills       |魔法スキル|
|menuCommands      |メニューコマンド|
|optAutosave       |オートセーブを有効化|
|optDisplayTp      |ウィンドウにTPを表示|
|optDrawTitle      |ゲームタイトルの描画|
|optExtraExp       |控えメンバーも経験値を獲得|
|optFloorDeath     |床タメージで戦闘不能|
|optFollowers      |パーティの隊列歩行|
|optKeyItemsNumber |大事なものの個数を表示|
|optSideView       |戦闘画面(サイドビュー)|
|optSlipDeath      |スリップダメージで戦闘不能|
|optTransparent    |透明状態で開始|
|partyMembers      |初期パーティ|
|ship              |大型船|
|skillTypes        |スキルタイプ|
|sounds            |効果音|
|startMapId        |初期位置の設定(マップID)|
|startX            |初期位置の設定(X座標)|
|startY            |初期位置の設定(Y座標)|
|switches          |スイッチ|
|terms             |用語|
|testBattlers      |戦闘テスト(パーティ)|
|testTroopId       |戦闘テスト(敵グループ)|
|title1Name        |タイトル画面(画像1)|
|title2Name        |タイトル画面(画像2)|
|titleBgm          |音楽(タイトルBGM)|
|titleCommandWindow|タイトル画面(コマンドウィンドウ)|
|variables         |変数|
|versionId         |バージョンID|
|victoryMe         |音楽(勝利ME)|
|weaponTypes       |武器タイプ|
|windowTone        |ウィンドウカラー|
