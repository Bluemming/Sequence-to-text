<h4 align='center'> 한국데이터정보과학회지 게재 논문 </h4>
<h2 align='center'> Sequence-to-text 기법을 활용한

언어 모델의 분류 성능 비교
<h3 align='center'> Comparison of Classification Performance of

Language Models using Sequence-to-Text Techniques </h3>


<br>   
<div align='center'>
<table>
    <thead>
        <tr>
            <th colspan="4"> First Author </th>
        </tr>
    </thead>
    <tbody>
        <tr>
          <tr>
            <td align='center'><a href="https://github.com/mixk0n9"><img src="https://github.com/mixk0n9.png" width="100" height="100"></td>
            <td align='center'><a href="https://github.com/ymk713"><img src="https://github.com/ymk713.png" width="100" height="100"></td>
            <td align='center'><a href="https://github.com/Bluemming"><img src="https://github.com/Bluemming.png" width="100" height="100"></td>
            <td align='center'><a href="https://github.com/iwantpubao"><img src="https://github.com/iwantpubao.png" width="100" height="100"></td>
          <tr>
            <td align='center'>김민경</td>
            <td align='center'>김유미</td>
            <td align='center'>민지현</td>
            <td align='center'>성현수</td>
          </tr>
        </tr>
    </tbody>
</table>

</div>


<!-- Using HTML to center the abstract -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Abstract</h2>
        <div class="content has-text-justified">
 최근 들어 활발한 언어 모형의 개발과 함께 많은 분야의 연구자들이 이에 관심을 갖게 되었다. 
언어 모형의 사용처는 매우 다양하여 많은 분야에 사용될 수 있다. 전통적인 통계학이나 머신러닝의 
분야에서는 기존에 이진 분류에 대한 연구가 활발하게 진행되어왔고, 언어 모형들 역시 동일한 과제를 수행할 
수 있다. 언어 모형의 특징으로 인해 입력 데이터는 테이블 형식의 숫자로 이루어진 데이터가 아니라 
문자형 식의 변수를 요구한다. 이 논문에서는 열 가지의 최신 언어 모형들의 목적과 특징들을 소개한다. 
한편, 언어 모형의 데이터 입력을 위해 시퀀스 데이터를 텍스트로 변환하는 sequence-to-text 방법의 
여러 가지 예시를 구체적으로 제시한다. 이를 통해 언어 모형 구현에 경험이 없는 독자들에게는 도움이 
될 것으로 기대한다. 마지막으로, 제시한 여러 가지 sequence-to-text 방법을 실제 데이터를 이용한 모의 
실험을 통하여 이 논문에서 소개하는 최신 언어 모형들의 성능을 비교하고 머신러닝 모형들의 결과도 
함께 제공하여 언어 모형들의 우수한 분류 성능을 확인한다.
        </div>
    </div>
</div>

---

## Background
활발한 언어 모형의 개발이 진행되고 있으며 다양한 분야에 사용될 수 있습니다. 전통적인 통계학이나 머신러닝 분야에서는 이진 분류에 대한 연구가 활발하게 진행되어왔고, 언어 모형들 역시 동일한 과제를 수행 가능합니다.

## Objective
이 논문에서의 주요 목표는 시계열 데이터의 패턴을 언어 모델로 학습하고 분류 예측에 사용하는 것입니다.


## Key Ideas
1. 연속된 시계열 데이터를 시퀀스 형태로 나열한 후 언어 모델이 이해할 수 있는 텍스트 형태로 변환합니다.
2. 단순히 순차적 행동을 텍스트로 나열하는 것이 아니라, 요약 정보를 문장 초두에 함께 제시합니다.
3. 사전 학습된 언어 모델을 HuggingFace로부터 불러와 분류 과제를 학습하여 예측을 수행합니다.
4. 동일한 정보량이 주어졌을 때, 언어 모델과 머신러닝 모델의 예측 성능을 비교합니다.

<p align="center">
  <img src="./images/preprocess_figure1.png" alt="sequence-to-text" width="800"/>
</p>
<p align="center">
    *Figure 1: Data preprocessing from sequence to text. Source: [논문링크](link).*
</p>

## Table: Comparison of Language models and Machine learning models

|  Score\Model  | BERT(scenario 4) | XGBoost(scenario 1) |
| ------------  | ---------------- | ------------------- |
|  F1-score  | 0.7363 | 0.6982 |
|  Precision | 0.6661 | 0.6153 |
|   Recall   | 0.8246 | 0.8075 |
|  Accuracy  | 0.7049 | 0.6511 |

## Significance
첫번째 시나리오를 통해 언어 모델이 머신러닝 모델과 비슷한 성능을 보이고, 그 이외의 시나리오에서 더 우수한 분류 성능을 보여주어 언어 모형들의 예측 능력이 뛰어남을 확인하였다.

## Citation
```
@article{?,
  title={Comparison of Classification Performance of Language Models using Sequence-to-Text Techniques},
  author={Kim, M., Kim, Y., Min, J., Seong, H., and Jung, Y.},
  journal={Journal of the Korean Data & Information Science Society.},
  volume={35},
  number={6},
  pages={815-834 (20 pages)},
  year={2024}
}
```
