# ASRLab 成功大學碩博士用畢業論文 LaTex 模版

此模板由專案 [ncku-thesis-template-latex](https://github.com/wengan-li/ncku-thesis-template-latex) 修改而來，原專案中有詳細的論文說明。(但可能過時，請以校方最新公告為主)

主要修改：

* 集合各段落成一個檔案，減少切換檔案的麻煩及方便修改中進行編譯。
* 減少過度包裝的 API 使用，以 Latex 原生 API 為主。
* 方便好用懶人包。

注意事項：

* `oral.tex` 原先用來產生學位考試論文證明，但已改成學校系統產生
* 浮水印部分會由圖書館統一生成，繳交檔案不得有浮水印
* 使用 "資訊工程學系" 而不是 "資訊工程研究所" 或其他

---

## 使用方法

```bash
git clone https://github.com/nckuasrlab/ASRLab_Thesis_Template.git --depth 1
```

產生 thesis.pdf 後建議把它加進 git 中，以便管理論文版本。

```bash
git add thesis/thesis.pdf -f
```

### Linux

```bash
# prerequisite
$ sudo apt-get install texlive-full texmaker
$ cd ASRLab_Thesis_Template/thesis

# compile and generate thesis PDF
$ make

# make outer cover
$ make cover

# generate example case
$ make example

# generate oral consent
$ make oral

# edit
$ make edit

# clean
$ make clean
```

### Windows

* 環境設定及安裝相依性套件
  * [Strawberry Perl](https://strawberryperl.com/)，選 64-bit 版本
  * [MikTeX](https://miktex.org/download)
  * VSCode (`james-yu.latex-workshop`, `analytic-signal.preview-pdf`)
  * 詳細請參考 [Use VSCode to Write LaTeX Paper](https://aben20807.github.io/posts/20210811-use-vscode-to-write-latex-paper/)
* 產生 PDF 檔案
  * thesis.tex 使用 Recipe: Compile
  * 封面 (`outer_cover.tex`) 使用 Recipe: Single

---

## 其他 Sample 樣板/範例

* [PDF 樣版/範例](https://github.com/wengan-li/ncku-thesis-template-latex-sample)
* [原作者 wengan-li 提供之模板](https://github.com/wengan-li/ncku-thesis-template-latex)
* [lycsjm 提供之模板](https://github.com/lycsjm/nckuthesis)
* 基本語法: [Latex Examples](https://aben20807.github.io/posts/20221227-latex-examples/)
* [Latex 符號手寫辨識](http://detexify.kirelabs.org/classify.html)

---

## License 授權條款

本著作採用創用 CC 姓名標示-非商業性-相同方式分享 4.0 授權條款

This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.

<p align="center">
  <img src='https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png' alt="CC-BY-NC-SA-4.0"/>
</p>

詳細[請看LICENSE](https://github.com/wengan-li/ncku-thesis-template-latex/blob/master/LICENSE)這檔案中的條款說明.

而本模版所使用到的國立成功大學浮水印則由國立成功大學擁有**所有**相關的權利. 故如使用這浮水印到論文以外的應用, 請跟'成大圖書館 系統管理組-數位論文小組'聯絡.
