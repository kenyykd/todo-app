<template>
  <a
    class="btn font-bold bg-gray-600 text-amber-50 mr-5"
    onclick="signin.showModal()"
    >登入</a
  >
  <dialog id="signin" class="modal">
    <div class="modal-box flex flex-col items-center">
      <h3 class="mb-7 text-2xl font-bold">登入</h3>
      <label class="input validator min-w-64 mb-0">
        <svg
          class="h-[1em] opacity-50"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
        >
          <g
            stroke-linejoin="round"
            stroke-linecap="round"
            stroke-width="2.5"
            fill="none"
            stroke="currentColor"
          >
            <path d="M19 21v-2a4 4 0 0 0-4-4H9a4 4 0 0 0-4 4v2"></path>
            <circle cx="12" cy="7" r="4"></circle>
          </g>
        </svg>
        <input
          type="text"
          required
          placeholder="Username"
          pattern="[A-Za-z][A-Za-z0-9\-]*"
          minlength="3"
          maxlength="30"
          title="Only letters, numbers or dash"
        />
      </label>
      <p class="validator-hint">
        Must be 3 to 30 characters
        <br />containing only letters, numbers or dash
      </p>
      <!-- password -->
      <label class="input validator min-w-64 mb-4">
        <svg
          class="h-[1em] opacity-50"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
        >
          <g
            stroke-linejoin="round"
            stroke-linecap="round"
            stroke-width="2.5"
            fill="none"
            stroke="currentColor"
          >
            <path
              d="M2.586 17.414A2 2 0 0 0 2 18.828V21a1 1 0 0 0 1 1h3a1 1 0 0 0 1-1v-1a1 1 0 0 1 1-1h1a1 1 0 0 0 1-1v-1a1 1 0 0 1 1-1h.172a2 2 0 0 0 1.414-.586l.814-.814a6.5 6.5 0 1 0-4-4z"
            ></path>
            <circle cx="16.5" cy="7.5" r=".5" fill="currentColor"></circle>
          </g>
        </svg>
        <input
          type="password"
          required
          placeholder="Password"
          minlength="8"
          pattern="(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,}"
          title="Must be more than 8 characters, including number, lowercase letter, uppercase letter"
        />
      </label>
      <p class="validator-hint hidden">
        Must be more than 8 characters, including
        <br />At least one number <br />At least one lowercase letter <br />At
        least one uppercase letter
      </p>
      <!--  -->
      <div class="modal-action">
        <form method="dialog">
          <button class="btn">關閉</button>
        </form>
        <button class="btn bg-gray-600 text-amber-50 submit">登入</button>
      </div>
    </div>
  </dialog>
</template>
