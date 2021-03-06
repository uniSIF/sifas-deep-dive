# 属性一致

アピールするスクールアイドルの属性が楽曲の属性と一致している場合、獲得ボルテージが属性一致補正されます。属性一致時は、アピールによる獲得ボルテージが1.2倍になります。

## 属性一致による獲得ボルテージ補正の計算

属性一致により補正された獲得ボルテージは、次のルールで計算されます。

1. 作戦効果（Vo）を適用した獲得ボルテージに、属性一致による補正量を乗算する。
2. 1.の計算結果の小数点以下を切り捨てて整数にする。

計算を数式で表すと、次のとおりとなります。

$$
v_{\text{at}} = \lfloor c_{\text{at}}v_{\text{tvo}}\rfloor
$$

$$
c_{\text{at}} = 
\begin{cases}
  1.2 & (\text{属性一致時})\\
  1 & (\text{属性不一致時})
\end{cases}
$$

ここで、数式内の変数の意味は次のとおりです。

$$
\begin{align}
  v_{\text{at}}  &= \text{属性一致を適用した獲得ボルテージ}\\
 v_{\text{tvo}} & = \text{作戦効果（Vo）を適用した獲得ボルテージ} \\
  c_{\text{at}} &= \text{属性一致による補正量}
\end{align}
$$

## 計算の例

前項の例を引き続き使用して、属性一致による補正を適用した獲得ボルテージを計算します。

![](../../.gitbook/assets/fig1-3-4a_base_appeal_increase_calc.jpg)

この編成の梨子が、「ユメノトビラ」上級で作戦効果（Vo）の効果を受けたときの獲得ボルテージは8015でした。ここで、梨子の属性は「ユメノトビラ」と同じピュアであるため、属性一致補正により獲得ボルテージが1.2倍され、9618となります。

$$
\begin{align}
v_{\text{at}} &= \lfloor 1.2v_{\text{tvo}}\rfloor\\
&=\lfloor 1.2 \times 8015 \rfloor\\
&= 9618
\end{align}
$$

{% hint style="info" %}
この計算結果とゲーム内の獲得ボルテージが等しくなることは「残スタミナ」の項で確認します。
{% endhint %}

