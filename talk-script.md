# Bidirectional Quadratic Voting: Leveraging Issue-Based Matching

## スライド1: タイトルスライド / Title Slide

こんにちは、皆さん。私はGMOペパボの栗林健太郎です。ETHTokyoがこのように盛大に開催されたことについて、スポンサー企業としてお慶び申し上げます。ところで、昨日までハッカソンが行われていたので、私も少しハックしてきました。スマートコントラクトを書くところまではいけませんでしたが、今日はその成果について簡単にお話しします。

Hello everyone. I'm Kentaro Kuribayashi from GMO Pepabo. As a sponsor, we're delighted to see ETHTokyo held on such a grand scale. By the way, there was a hackathon until yesterday, so I did some hacking too. I didn't get as far as writing smart contracts, but today I'll briefly talk about what I came up with.

## スライド2: 自己紹介 / About Me

私はGMOペパボのCTOを務めています。日本の友人は私のことを「あんちぽ」と呼んでいます。ぜひ皆さんも「あんちぽ」と気軽にお呼びください。

I'm the CTO of GMO Pepabo. Please feel free to call me "Anchipo".

## スライド3: 免責事項 / Disclaimer

始める前に、この発表は私の所属組織の見解を代表するものではなく、また私個人の政治的意見を反映するものでもないことをお断りしておきます。

Before we begin, I'd like to clarify that this presentation does not represent the views of my affiliated organization, nor does it reflect my personal political opinions.

## スライド4: 課題：投票のジレンマ (1/2) / Challenge: The Voting Dilemma (1/2)

選挙における大きな課題の一つは、候補者選択において経験と革新のバランスをとることです。例えば、経験豊富で有力な候補が複数いる場合で、かつ、テクノロジーを専門とする新人候補がいる場合に、どのように投票するかという問題です。東京に住んでいる方の中には、最近そういうジレンマに直面した方もいらっしゃるかもしれません。

A big challenge in elections is balancing experience and new ideas when choosing candidates. For example, it's hard to decide how to vote when there are several experienced, strong candidates and also a new candidate who specializes in technology. Some people living in Tokyo might have faced this dilemma recently.

## スライド5: 課題：投票のジレンマ (2/2) / Challenge: The Voting Dilemma (2/2)

過去の実績に焦点を当てすぎると、新しいアイデアの認識が妨げられる可能性があります。一方で、新しいアイデアを優先すると、現実的には対立候補を有利にしてしまう可能性があります。

Focusing too much on past achievements might hinder recognition of new ideas. On the other hand, prioritizing new ideas may unintentionally favor opposing candidates in reality.

## スライド6: 二次投票（QV） / Quadratic Voting (QV)

この問題の潜在的な解決策として、二次投票（QV）があります。QVは有権者が分散した選好を表現することを可能にし、単一の候補者を選ぶことに限定されません。

Quadratic Voting (QV) is a potential solution to this problem. QV allows voters to express distributed preferences and is not limited to choosing a single candidate.

## スライド7: 選挙へのQVの適用 / Applying QV to Elections

このスライドは、選挙にQVを適用する方法を示しています。有権者は候補者に対してQVによって投票します。もっともスコアの高い候補者が当選します。

This slide shows how QV works in elections. Voters use QV to vote for candidates. The candidate with the highest score wins.

## スライド8: さらに一歩進んで / Taking It a Step Further

しかし、選挙におけるQVでも、有権者は候補者の真の選好について不確実なままです。人に投票するのではなく、具体的な課題に基づいて有権者と候補者を一致させる投票方法が必要です。

But even with QV in elections, voters still don't know what candidates really want. We need a way to vote that matches voters and candidates based on specific issues, not just voting for people.

## スライド9: 双方向二次投票（BQV） / Bidirectional Quadratic Voting (BQV)

そこで、双方向二次投票（BQV）を提案します。このスライドは、選挙にBQVを適用する方法を示しています。BQVでは、候補者も有権者もともに、具体的なイシューに対してQVによって投票します。そして、候補者の投票結果と有権者の投票結果の類似度を計算することで、有権者の選好にもっとも近い候補者が当選します。

So, I propose Bidirectional Quadratic Voting (BQV). This slide shows how BQV works in elections. In BQV, both candidates and voters use QV to vote on specific issues. We then compare the voting results of candidates and voters. The candidate whose votes are most similar to the voters' preferences wins.

## スライド10: BQVの主な特徴 / Key Features of BQV

BQVはマッチングアプリのメカニズムに似ていますが、1対Nのマッチングではなく、N対Mのマッチングを可能にします。投票システムとしては複雑ですが、理解可能である必要があります。

BQV resembles a matching app mechanism, but unlike 1:N matching in dating apps, BQV facilitates N:M matching. As a voting system, it needs to be comprehensible, though it's still a bit complicated.

## スライド11: シミュレーションのセットアップ / Simulation Setup

さて、BQVの効果を検証するために、シミュレーションを行いました。このスライドはシミュレーションのセットアップと主な前提条件を示しています。ただし、これらの設定は実際の選挙をシミュレートするには不十分であり、恣意的な仮定を含んでいることにご注意ください。これらは参考程度にとどめるべきです。

To verify the effectiveness of BQV, we conducted simulations. This slide shows the simulation setup and key assumptions. However, please note that these settings are insufficient to simulate an actual election and contain arbitrary assumptions. They should be considered for reference purposes only.

## スライド12: 候補者の選好 / Candidate Preferences

シミュレーションでは、政治的スペクトラムにわたる候補者を想定しました。候補者1と4は比較的政治経験が高く、候補者2は技術の専門家としています。

In our simulation, we assumed candidates spanning the political spectrum. Candidates 1 and 4 have relatively high political experience, while Candidate 2 is a tech expert.

## スライド13: 有権者の分布 / Voter Distribution

有権者の分布として、正規分布、二峰性分布、左偏分布、右偏分布の4つを仮定し、それぞれについてシミュレーションを行いました。

We assumed four voter distributions: normal, bimodal, left-skewed, and right-skewed, and conducted simulations for each distribution.

## スライド14: シミュレーション結果 (1/2) / Simulation Results (1/2)

このスライドは、シミュレーションの結果を示しています。QV/BQVは現状行われている投票方式と比較して、より均衡のとれた選好を反映しています。政治実績を重視しつつ、専門性を投票結果に反映できている可能性があります。そのため、先に述べたジレンマを解決するかもしれません。

This slide shows our simulation results. QV/BQV gives more balanced voter preferences than regular voting. It may value political experience while also considering expertise. This could solve the dilemma we mentioned earlier.

## スライド15: シミュレーション結果 (2/2) / Simulation Results (2/2)

ただし、より正確なシミュレーションにはより精密なモデリングが必要です。シミュレーションの詳細は私のGitHubリポジトリをご参照ください。

However, more precise modeling is needed for more accurate simulations. For complete simulation details, please refer to my GitHub repository.

## スライド16: 結論 / Conclusion

QV/BQVはEthereumでの社会実装に有望なメカニズムです。GMOはEthereumコミュニティと協力して、ポジティブな社会的影響を創出することを目指しています。ブロックチェーン技術を活用して、より良い世界を構築できると信じています。

QV/BQV is a promising mechanism for social implementation on Ethereum. GMO aims to collaborate with the Ethereum community to create positive social impact. We believe that together, we can leverage blockchain technology to build a better world!

Thank you for your attention.