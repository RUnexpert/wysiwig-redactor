<template>
  <div>
    <div class="toolbar">
      <the-button @click="undo" title="Назад">
        <svg
          width="22"
          height="20"
          viewBox="0 0 22 20"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M18.6358 19.5824C18.3582 19.86 17.9929 20 17.6299 20C17.2645 20 16.8992 19.86 16.6216 19.5824C16.0664 19.0249 16.0664 18.1257 16.6216 17.5682C19.7604 14.4294 19.7604 9.32384 16.6216 6.18505C13.4852 3.04864 8.37722 3.04864 5.24081 6.18505L4.72598 6.69988H8.12337C8.90866 6.69988 9.54686 7.33808 9.54686 8.12337C9.54686 8.91103 8.90866 9.54686 8.12337 9.54686H1.42349C0.638197 9.54686 0 8.91103 0 8.12337V1.42349C0 0.638197 0.638197 0 1.42349 0C2.20878 0 2.84697 0.638197 2.84697 1.42349V4.55279L3.22657 4.17319C7.47568 -0.0759193 14.3867 -0.0759193 18.6358 4.17319C22.8849 8.4223 22.8849 15.3333 18.6358 19.5824Z"
            fill="#639EFF"
          />
        </svg>
      </the-button>
      <the-button @click="redo" title="Вперед"
        ><svg
          width="22"
          height="20"
          viewBox="0 0 22 20"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M3.18684 19.5824C3.46442 19.86 3.82978 20 4.19277 20C4.55813 20 4.92349 19.86 5.20107 19.5824C5.75624 19.0249 5.75624 18.1257 5.20107 17.5682C2.06229 14.4294 2.06229 9.32384 5.20107 6.18505C8.33749 3.04864 13.4454 3.04864 16.5819 6.18505L17.0967 6.69988H13.6993C12.914 6.69988 12.2758 7.33808 12.2758 8.12337C12.2758 8.91103 12.914 9.54686 13.6993 9.54686H20.3992C21.1845 9.54686 21.8227 8.91103 21.8227 8.12337V1.42349C21.8227 0.638197 21.1845 0 20.3992 0C19.6139 0 18.9757 0.638197 18.9757 1.42349V4.55279L18.5961 4.17319C14.347 -0.0759193 7.43595 -0.0759193 3.18684 4.17319C-1.06227 8.4223 -1.06227 15.3333 3.18684 19.5824Z"
            fill="#639EFF"
          />
        </svg>
      </the-button>
      <the-button @click="setHeading" title="Заголовок"
        ><svg
          width="20"
          height="23"
          viewBox="0 0 20 23"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M20 1.5V4.0075C20 4.8375 19.3317 5.5075 18.5037 5.5075C17.6783 5.5075 17.0075 4.8375 17.0075 4.0075V3H11.4963V20H12.8454C13.6733 20 14.3416 20.6725 14.3416 21.5C14.3416 22.3275 13.6733 23 12.8454 23H7.15461C6.32668 23 5.65835 22.3275 5.65835 21.5C5.65835 20.6725 6.32668 20 7.15461 20H8.50374V3H2.99252V4.0075C2.99252 4.8375 2.3217 5.5075 1.49626 5.5075C0.668329 5.5075 0 4.8375 0 4.0075V1.5C0 0.6725 0.668329 0 1.49626 0H18.5037C19.3317 0 20 0.6725 20 1.5Z"
            fill="#639EFF"
          />
        </svg>
      </the-button>
      <the-button @click="setParagraph" title="Абзац"
        ><svg
          width="13"
          height="14"
          viewBox="0 0 13 14"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M12.4876 1.74158V3.06038C12.4876 3.98719 11.7344 4.74039 10.8076 4.74039C10.004 4.74039 9.332 4.17479 9.1668 3.42159H8.0048V10.5868C8.8476 10.6792 9.5056 11.3932 9.5056 12.2584C9.5056 13.188 8.7524 13.9384 7.8256 13.9384H4.824C3.89439 13.9384 3.14399 13.188 3.14399 12.2584C3.14399 11.3932 3.7992 10.6792 4.64479 10.5868V3.42159H3.48C3.3148 4.17479 2.6428 4.74039 1.8392 4.74039C0.912395 4.74039 0.159195 3.98719 0.159195 3.06038V1.74158C0.159195 0.811985 0.912395 0.0615845 1.8392 0.0615845H10.8076C11.7344 0.0615845 12.4876 0.811985 12.4876 1.74158Z"
            fill="#639EFF"
          />
        </svg>
        <svg
          width="13"
          height="14"
          viewBox="0 0 13 14"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M12.4876 1.74158V3.06038C12.4876 3.98719 11.7344 4.74039 10.8076 4.74039C10.004 4.74039 9.332 4.17479 9.1668 3.42159H8.0048V10.5868C8.8476 10.6792 9.5056 11.3932 9.5056 12.2584C9.5056 13.188 8.7524 13.9384 7.8256 13.9384H4.824C3.89439 13.9384 3.14399 13.188 3.14399 12.2584C3.14399 11.3932 3.7992 10.6792 4.64479 10.5868V3.42159H3.48C3.3148 4.17479 2.6428 4.74039 1.8392 4.74039C0.912395 4.74039 0.159195 3.98719 0.159195 3.06038V1.74158C0.159195 0.811985 0.912395 0.0615845 1.8392 0.0615845H10.8076C11.7344 0.0615845 12.4876 0.811985 12.4876 1.74158Z"
            fill="#639EFF"
          />
        </svg>
      </the-button>
      <the-button @click="insertImage" title="Вставить картинку"
        ><svg
          width="22"
          height="20"
          viewBox="0 0 22 20"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M20.5652 0.0784912H1.43478C0.643261 0.0784912 0 0.721752 0 1.51327V18.4868C0 19.2783 0.643261 19.9215 1.43478 19.9215H20.5652C21.3567 19.9215 22 19.2783 22 18.4868V1.51327C22 0.721752 21.3567 0.0784912 20.5652 0.0784912ZM19.1304 17.052H2.86957V16.3274L5.94956 13.2474L7.38674 14.6822C7.9463 15.2441 8.855 15.2441 9.41457 14.6846L15.0843 9.0148L19.1304 13.0609V17.052ZM19.1304 9.00523L16.0983 5.97067C15.5363 5.4111 14.63 5.4111 14.068 5.97067L8.40065 11.6404L6.96348 10.2033C6.40391 9.64371 5.49522 9.64371 4.93565 10.2033L2.86957 12.2694V2.94806H19.1304V9.00523Z"
            fill="#639EFF"
          />
        </svg>
      </the-button>
      <the-button @click="copyHTML" title="Скопировать HTML"
        >Скопировать HTML</the-button
      >
    </div>
    <div
      class="editor"
      ref="editor"
      contenteditable="true"
      @input="saveHistory"
    >
      <p>
        Таким образом консультация с широким активом представляет собой
        интересный эксперимент проверки позиций, занимаемых участниками в
        отношении поставленных задач. С другой стороны постоянное
        информационно-пропагандистское обеспечение нашей деятельности
        представляет собой интересный эксперимент проверки форм развития.
        Идейные соображения высшего порядка, а также укрепление и развитие
        структуры влечет за собой процесс внедрения и модернизации
        соответствующий условий активизации. Задача организации, в особенности
        же реализация намеченных плановых заданий играет важную роль в
        формировании дальнейших направлений развития. Повседневная практика
        показывает, что постоянное информационно-пропагандистское обеспечение
        нашей деятельности играет важную роль в формировании существенных
        финансовых и административных условий.
      </p>
      <h2>Смотрите какие бибизянки</h2>
      <img
        src="https://s3-alpha-sig.figma.com/img/41f2/0008/69cac4e6271b50281c7941f0ba76b675?Expires=1734307200&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=VI7DsfUdDcL7ntsbYp020x1dowzPdhxYRon1ZruybbZX7XFW3OE2VbculqjF8FEe6SVDGhwrev~K5DsZtVnxiR~80rKtFG1P6oNDFicczBHXKLh0WhIlkhgbsxLpk89tkJgJnqknYMgrbWIPn6lgI-DD2l1UDxQZjtX0OsNcBivL44ESmSaQ6qty0Zcqqa89un2urVjinX9N2QExAA21kLEczEVvKQ9MUZN45Gy6zo8x2wAy8rq17a6IaZ5FJtfCzyY2uqzgOmf0p4VeTGD6sn5mNDlnKs7oc7Sw4p6txMfKSKpXYT3ueRAaZkObibFRKHFIELy1uO0bRbT~s~3ChA__"
        alt="Бибизяны"
      />
      <p>
        Таким образом консультация с широким активом представляет собой
        интересный эксперимент проверки позиций, занимаемых участниками в
        отношении поставленных задач. С другой стороны постоянное
        информационно-пропагандистское обеспечение нашей деятельности
        представляет собой инйцу шо шщйоц ущойц ущошцщйуо йцщуо йщцоу щйоу
        шщйцош ущйтересный эксперимент проверки форм развития. Идейные
        соображения высшего порядка, а также укрепление и развитие структуры
        влечет за собой процесс внедрения и модернизации соответствующий условий
        активизации. Задача организации, в особенности же реализация намеченных
        плановых заданий играет важную роль в формировании дальнейших
        направлений развития. Повседневная практика показывает, что постоянное
        информационно-пропагандистское обеспечение нашей деятельности играет
        важную роль в формировании существенных финансовых и административных
        условий. Товарищи! новая модель организационной деятельности требуют от
        нас анализа направлений прогрессивного развития. Задача организации, в
        особенности же постоянный количественный рост и сфера нашей активности
        требуют от нас анализа позиций, занимаемых участниками в отношении
        поставленных задач. Задача организации, в особенности же реализация
        намеченных плановых заданий требуют от нас анализа системы обучения
        кадров, соответствует насущным потребностям.
      </p>
    </div>
  </div>
</template>

<script>
import TheButton from "./TheButton.vue";
export default {
  name: "TheEditor",

  components: {
    TheButton,
  },

  data() {
    return {
      history: [],
      historyIndex: -1,
    };
  },

  methods: {
    saveHistory() {
      const editor = this.$refs.editor;
      if (editor) {
        const content = editor.innerHTML;
        if (this.historyIndex < this.history.length - 1) {
          this.history.splice(this.historyIndex + 1);
        }
        this.history.push(content);
        this.historyIndex++;
      }
    },

    undo() {
      if (this.historyIndex > 0) {
        this.historyIndex--;
        this.updateEditorContent(this.history[this.historyIndex]);
      }
    },

    redo() {
      if (this.historyIndex < this.history.length - 1) {
        this.historyIndex++;
        this.updateEditorContent(this.history[this.historyIndex]);
      }
    },

    setHeading() {
      this.toggleBlock("h2");
    },

    setParagraph() {
      this.toggleBlock("p");
    },

    toggleBlock(tag) {
      const selection = window.getSelection();
      const range = this.getRange();
      if (!range) {
        const newElement = document.createElement(tag);
        newElement.textContent = "Новый блок";
        this.$refs.editor.appendChild(newElement);
        this.saveHistory();
        return;
      }

      const parentBlock = this.findParentBlock(range.startContainer);
      if (parentBlock && parentBlock.tagName.toLowerCase() !== "div") {
        if (parentBlock.tagName.toLowerCase() !== tag) {
          this.replaceTag(parentBlock, tag);
          this.saveHistory();
        }
      } else {
        const newElement = document.createElement(tag);
        range.surroundContents(newElement);
        this.saveHistory();
      }
    },

    findParentBlock(node) {
      while (node && node.nodeType !== Node.ELEMENT_NODE) {
        node = node.parentNode;
      }
      return node && node.tagName !== "DIV" ? node : null;
    },

    replaceTag(node, newTag) {
      const newNode = document.createElement(newTag);
      newNode.innerHTML = node.innerHTML;
      node.parentNode.replaceChild(newNode, node);
    },

    getRange() {
      const selection = window.getSelection();
      if (selection.rangeCount > 0) {
        return selection.getRangeAt(0);
      }
      return null;
    },

    updateEditorContent(content) {
      const editor = this.$refs.editor;
      if (editor) {
        editor.innerHTML = content;
      }
    },

    insertImage() {
      const url = prompt("Введите URL изображения:");
      if (url) {
        const img = document.createElement("img");
        img.src = url;
        img.alt = "Вставленное изображение";

        const range = this.getRange();
        const editor = this.$refs.editor;

        if (range && editor.contains(range.startContainer)) {
          range.collapse(false);
          range.insertNode(img);
          console.log(1);
        } else {
          editor.appendChild(img);
          console.log(editor);
        }

        this.saveHistory();
      }
    },
    copyHTML() {
      const editor = this.$refs.editor;
      if (editor) {
        const content = editor.innerHTML;
        navigator.clipboard.writeText(content).then(
          () => alert("HTML скопирован в буфер обмена!"),
          () => alert("Не удалось скопировать HTML."),
        );
      }
    },
  },

  mounted() {
    this.saveHistory();
  },
};
</script>

<style>
.toolbar {
  display: flex;
  gap: 10px;
  margin-bottom: 10px;
}

.editor {
  padding: 10px 20px;
  min-height: 300px;
  background-color: rgba(0, 0, 0, 0.184);
  border-radius: 5px;
  overflow: auto;
  outline: 0;
}

p,
img,
h2 {
  padding: 10px 0;
}

img {
  display: block;
  max-height: 500px;
  max-width: 100%;
}
</style>
