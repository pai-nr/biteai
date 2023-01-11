# 기본 개발 가이드
## 개발 프로세스
```{note}
추후 작성 예정입니다. 
```
## 개발 가이드
```{note}
지속 업데이트 될 예정입니다. 
```
- 주피터북의 내용은 Jupyter Notebooks (`.ipynb`) 또는 마크다운 (`.md`) 파일로 작성할 수 있음 
- 두 가지 파일은 마크다운 중에서도 **MyST Markdown** 양식에 따라 작성할 수 있음
- MyST의 신택스를 보여주는 샘플 파일로 이 파일을 작성함

## What is MyST?

- MyST 는 "Markedly Structured Text"의 약어로, **roles** 와 **directives** 관련하여 파이썬 문서화 라이브러리인 Sphinx에서 사용하는 여러 신택스를 활용할 수 있도록 만들어짐
- MyST 자세히 알아보기 [the MyST Markdown Overview](https://jupyterbook.org/content/myst.html).

## Sample Roles and Directives
- Roles과 directives는 주피터 북에서 가장 강력한 두 가지 도구임
- 마크업 언어로 작성하되, 함수처럼 사용이 가능함
- **roles 는 보통 한 줄로 작성**되는 반면, **directives는 여러 줄**로 작성
- 다양한 형식의 입력값을 수용하며 사전에 정의된 방식으로 입력값을 처리하여 보여줌

- 예시 1 : "note" directive
    - 책을 쓸 때 특별히 박스를 쳐서 작성해야 하는 내용을 적을 수 있음. 간단한 MyST 문법으로 이 박스를 만들어서 작성할 수 있음 
    ```{note}
    여기에 노트를 작성할 수 있습니다. 
    ```
    - 구현 방식 : 
    `` ```{note}``` ``

- 예시 2 : 같은 책 안의 챕터(마크다운 혹은 노트북 파일)인용하는 roles
   %-- - {doc}`markdown-notebooks`
    %- 대괄호 안에 'doc'라고 쓰고, `을 이용하여 파일 이름을 쓰면, 해당 파일의 h1으로 지정된 텍스트로 링크가 걸림
    %- 구현 방식 : 
    %`` {doc}`markdown-notebooks` ``
     %-->
- 예시 3 : 인용
    - 레퍼런스 인용은 `bibtex` 파일로 저장하여 활용할 수 있음
    - {cite}`holdgraf_evidence_2014`
    - 구현 방식 : 
    `` {cite}`holdgraf_evidence_2014` `` 
    - `reference.bib` 파일에 적혀있는 내용은 아래와 같음
    ``` 
    @inproceedings{holdgraf_evidence_2014,
        address = {Brisbane, Australia, Australia},
        title = {Evidence for {Predictive} {Coding} in {Human} {Auditory} {Cortex}},
        booktitle = {International {Conference} on {Cognitive} {Neuroscience}},
        publisher = {Frontiers in Neuroscience},
        author = {Holdgraf, Christopher Ramsay and de Heer, Wendy and Pasley, Brian N. and Knight, Robert T.},
        year = {2014}
    }
    ```

Moreover, you can insert a bibliography into your page with this syntax:
The `{bibliography}` directive must be used for all the `{cite}` roles to
render properly.
For example, if the references for your book are stored in `references.bib`,
then the bibliography is inserted with:

```{bibliography}
```

## Learn more

This is just a simple starter to get you started.
You can learn a lot more at [jupyterbook.org](https://jupyterbook.org).
