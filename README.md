
# nanoKONTROLの入力をいい感じに取れるやつ

## 前準備

MidiInの後ろにRenameを挟んで名前を変更します。

from `ch1clrl*` -> to `*`

## 本編

名前を変更したらそのまま`NanoKontrolAnalog`か`NanoKontrolBtn`に入力します。オペレーターの名前を変更するとChannel名も変わります。

パラメータは以下の通り

**共通**

- Track
    - 取得したいフェーダー / エンコーダー / ボタンが左から何番目のものか。0スタート。

**Analog**

- Rotary
    - エンコーダーの値を取得するか。オフにするとフェーダー。
- Range
    - 出力の範囲

**Btn**

- Name
    - Channelに付ける名前。スペース区切りでS, M, Rの順に入力。
- Index
    - オンで最後に押されたボタンのインデックスを出力する。Channel名はNameの一番最初のものが使われる。  
    ~~同時押しするとバグる~~