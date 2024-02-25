<script setup>
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <div class="w-full h-screen	bg-gradient-to-b from-pink-200 ... flex justify-center	items-center	flex-col">
      <div class="box w-2/3	h-3/4	bg-orange-50 p-2">
        <div class="enter">
          <input type="text" class="add-text w-4/5	h-7	">
          <button class="add-list">新增</button>
        </div>
        <div class="title-list h-12 flex justify-start	 items-center px-2">
          <div class="title w-20 h-10 bg-indigo-400 hover:bg-yellow-200 px-3 text-center leading-9 rounded-t" id="all" data-title="all-data">全部</div>
          <div class="title w-20 h-10 bg-indigo-400 hover:bg-yellow-200 px-3 text-center leading-9 mx-2 rounded-t	" id="do" data-title="do-data">已執行</div>
          <div class="title w-20 h-10 bg-indigo-400 hover:bg-yellow-200 px-3 text-center leading-9 rounded-t" id="yet" data-title="yet-data">未執行</div>
        </div>
        <div class="content-list w-full	 h-auto	 bg-teal-50	">
          <div class="content" data-content="all-data">
            <div class="in-title flex justify-between	 items-center">
              <span>執行</span>
              <span>事項</span>
              <span>功能</span>
            </div>
            <div class="in-tool">
              <!-- <input type="checkbox" name="" id=""> -->
              <div class="data-show"></div>

              <!-- <div>
                    <button class="set">編輯</button>
                    <button class="delete">刪除</button>
                </div> -->

            </div>
          </div>
          <div class="content hidden" data-content="do-data"></div>
          <div class="content hidden" data-content="yet-data"></div>
        </div>
      </div>

    </div>
  </main>
</template>
