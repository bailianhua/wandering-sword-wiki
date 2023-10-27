<script>
  import "../tailwind.css";
</script>

<header>
  <div class="navbar bg-base-100">
    <div class="flex-1">
      <a href="/" class="btn btn-ghost normal-case text-xl"
        >
        <div class="avatar">
          <div
            class="w-16 rounded-full"
          >
            <img src="/logo.png" />
          </div>
        </div>Wandering Sword Wiki</a
      >
    </div>
    <div class="flex-none gap-2">
      <div class="form-control">
        <input
          type="text"
          placeholder="Search"
          class="input input-bordered w-24 md:w-auto"
        />
      </div>
      <div class="dropdown dropdown-end">
        <label tabindex="0" class="btn btn-ghost btn-circle avatar">
          <div class="w-10 rounded-full">
            <img src="/images/stock/photo-1534528741775-53994a69daeb.jpg" />
          </div>
        </label>
        <ul
          tabindex="0"
          class="mt-3 z-[1] p-2 shadow menu menu-sm dropdown-content bg-base-100 rounded-box w-52"
        >
          <li>
            <a class="justify-between">
              Profile
              <span class="badge">New</span>
            </a>
          </li>
          <li><a>Settings</a></li>
          <li><a>Logout</a></li>
        </ul>
      </div>
    </div>
  </div>
</header>
<main>
  <div class="flex">
    <div class="flex-none w-1/6">
      <ul class="menu w-full rounded-box">
        <li><a href="aboutus">About us</a></li>
        <li>
          <details open>
            <summary>Parent</summary>
            <ul>
              <li><a>level 2 item 1</a></li>
              <li><a>level 2 item 2</a></li>
              <li>
                <details open>
                  <summary>Parent</summary>
                  <ul>
                    <li><a>level 3 item 1</a></li>
                    <li><a>level 3 item 2</a></li>
                  </ul>
                </details>
              </li>
            </ul>
          </details>
        </li>
        <li><a>Item 3</a></li>
      </ul>
    </div>
    <div class="flex-auto">
      <slot />
    </div>
  </div>
</main>
