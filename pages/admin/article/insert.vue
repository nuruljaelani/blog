<template>
  <div>
    <div class="flex min-h-screen">
      <div class="w-1/5">
        <div class="bg-white p-4 flex flex-col">
          <p class="font-bold text-2xl text-red-500 px-8 my-4">
            Admin
          </p>
          <div class="flex flex-col font-medium my-8 px-4">
            <div class="flex flex-col space-y-4">
              <div class="flex items-center space-x-2 bg-gray-200 rounded-md py-2 px-2">
                <fa-icon icon="home" />
                <p>Dashboard</p>
              </div>
              <div class="flex items-center space-x-2 py-2 px-2">
                <fa-icon icon="file" />
                <p>Articles</p>
              </div>
              <div class="flex items-center space-x-2 py-2 px-2">
                <fa-icon icon="user" />
                <p>Users</p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="w-4/5 bg-blue-50">
        <div class="flex flex-col space-y-8 py-8 px-8">
          <div class="flex bg-white py-2 shadow justify-end rounded-xl px-4">
            <div class="flex items-center space-x-2">
              <div class="flex bg-gray-200 rounded-full w-10 h-10" />
              <p class="font-medium">
                Admin
              </p>
            </div>
          </div>
          <p class="text-2xl text-blue-600 font-bold">
            Insert Article
          </p>
          <div class="bg-white shadow-md rounded-md">
            <div class="flex flex-col p-4">
              <form>
                <div class="flex flex-col space-y-2">
                  <label class="text-gray-600 font-medium">
                    Title
                  </label>
                  <input type="text" class="border appearance-none focus:outline-none rounded-md p-2">
                </div>
                <div class="flex flex-col space-y-2">
                  <label class="text-gray-600 font-medium">
                    Body
                  </label>
                  <div>
                    <client-only>
                      <quillEditor
                        ref="editor"
                        v-model="content"
                        :options="editorOption"
                        @blur="onEditorBlur($event)"
                        @focus="onEditorFocus($event)"
                        @ready="onEditorReady($event)"
                      />
                    </client-only>
                  </div>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { quillEditor } from 'vue-quill-editor/dist/ssr'
export default {
  name: 'QuillEditor',
  directives: {
    quill: quillEditor
  },
  data () {
    return {
      content: '<p>I am Example</p>',
      editorOption: {
        // Some Quill options...
        theme: 'snow',
        modules: {
          toolbar: [
            ['bold', 'italic', 'underline', 'strike'],
            ['blockquote', 'code-block']
          ]
        }
      }
    }
  },
  mounted () {
    // eslint-disable-next-line no-console
    console.log('App inited, the Quill instance object is:', this.$refs.editor.quill)
    setTimeout(() => {
      this.content = 'I was changed!'
    }, 3000)
  },
  methods: {
    onEditorBlur (editor) {
      // eslint-disable-next-line no-console
      console.log('editor blur!', editor)
    },
    onEditorFocus (editor) {
      // eslint-disable-next-line no-console
      console.log('editor focus!', editor)
    },
    onEditorReady (editor) {
      // eslint-disable-next-line no-console
      console.log('editor ready!', editor)
    }
  }
}
</script>
