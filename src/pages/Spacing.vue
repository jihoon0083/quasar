<template>
  <q-page class="q-pa-xl">
    <section class="q-mb-xl">
      <div class="text-h4">Spacing</div>
      <q-separator class="q-my-md" />
      <div class="bg-primary q-pa-sm q-mt-md">
        <div class="bg-dark text-white">
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repellendus,
          alias? Praesentium maiores illum nisi quisquam. Harum, nostrum
          repudiandae excepturi explicabo, corrupti quos ut eius vero cupiditate
          blanditiis numquam suscipit sed.
        </div>
      </div>
      <div class="bg-primary q-pa-md q-mt-md">
        <div class="bg-dark text-white">
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repellendus,
          alias? Praesentium maiores illum nisi quisquam. Harum, nostrum
          repudiandae excepturi explicabo, corrupti quos ut eius vero cupiditate
          blanditiis numquam suscipit sed.
        </div>
      </div>
      <div class="bg-primary q-pa-lg q-mt-md">
        <div class="bg-dark text-white">
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repellendus,
          alias? Praesentium maiores illum nisi quisquam. Harum, nostrum
          repudiandae excepturi explicabo, corrupti quos ut eius vero cupiditate
          blanditiis numquam suscipit sed.
        </div>
      </div>
      <div class="bg-primary q-pa-xl q-mt-md">
        <div class="bg-dark text-white">
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Repellendus,
          alias? Praesentium maiores illum nisi quisquam. Harum, nostrum
          repudiandae excepturi explicabo, corrupti quos ut eius vero cupiditate
          blanditiis numquam suscipit sed.
        </div>
      </div>
      <div
        class="bg-primary q-mt-md flex flex-center"
        style="width: 400px; height: 400px"
      >
        <div class="bg-dark text-white" style="width: 100px; height: 100px">
          Hello
        </div>
      </div>
    </section>
    <section class="q-mb-xl">
      <div class="text-h4">Components</div>
      <q-separator class="q-my-md" />
      <q-card
        class="my-card bg-secondary text-white q-mx-auto"
        style="width: 400px"
      >
        <q-card-section>
          <div class="text-h6">Our Changing Planet</div>
          <div class="text-subtitle2">by John Doe</div>
        </q-card-section>

        <q-card-section>
          {{ lorem }}
        </q-card-section>

        <q-separator dark />

        <q-card-actions>
          <q-btn padding="lg" outline>Action 1</q-btn>
          <q-btn padding="none" outline>Action 2</q-btn>
          <!--
          <q-btn class="q-pa-xl" outline>Action 3</q-btn>
          -->
        </q-card-actions>
      </q-card>

      <q-card class="my-card">
        <q-card-section>
          <div class="text-h6">Our Changing Planet</div>
          <div class="text-subtitle2">by John Doe</div>
        </q-card-section>

        <q-separator />

        <q-card-actions vertical>
          <q-btn flat>Action 1</q-btn>
          <q-btn flat>Action 2</q-btn>
        </q-card-actions>
      </q-card>

      <q-card class="my-card bg-purple text-white">
        <q-card-section>
          <div class="text-h6">Our Changing Planet</div>
          <div class="text-subtitle2">by John Doe</div>
        </q-card-section>

        <q-card-actions>
          <q-btn flat>Action 1</q-btn>
          <q-btn flat>Action 2</q-btn>
        </q-card-actions>
      </q-card>

      <q-card flat bordered class="my-card bg-grey-1">
        <q-card-section>
          <div class="row items-center no-wrap">
            <div class="col">
              <div class="text-h6">Our Planet</div>
              <div class="text-subtitle2">by John Doe</div>
            </div>

            <div class="col-auto">
              <q-btn color="grey-7" round flat icon="more_vert">
                <q-menu cover auto-close>
                  <q-list>
                    <q-item clickable>
                      <q-item-section>Remove Card</q-item-section>
                    </q-item>
                    <q-item clickable>
                      <q-item-section>Send Feedback</q-item-section>
                    </q-item>
                    <q-item clickable>
                      <q-item-section>Share</q-item-section>
                    </q-item>
                  </q-list>
                </q-menu>
              </q-btn>
            </div>
          </div>
        </q-card-section>

        <q-card-section>
          {{ lorem }}
        </q-card-section>

        <q-separator />

        <q-card-actions>
          <q-btn outline>Action 1</q-btn>
          <q-btn outline>Action 2</q-btn>
        </q-card-actions>
      </q-card>
    </section>
  </q-page>
</template>

<script setup></script>

<style lang="scss" scoped></style>
