<script>
  import { dragScroll } from '$lib/dragScroll';
  import Project from './Project.svelte';
</script>

<div class="max-w-4xl mx-auto px-4 py-8 grid gap-8">
  <div class="flex gap-8 justify-between items-center">
    <div class="space-y-2">
      <div class="flex gap-2 items-center">
        <h1>dllcrt0</h1>
        <a rel="external" href="https://github.com/dllcrt0" class="group">
          <img
            src="https://unpkg.com/simple-icons/icons/github.svg"
            alt="Github"
            class="h-5 w-5 group-hover:opacity-70 transition dark:invert"
          />
        </a>
      </div>
      <p>I mainly do software development and reverse engineering.</p>
    </div>

    <img
      src="https://avatars.githubusercontent.com/u/25990062"
      alt="Avatar"
      class="rounded-full aspect-square w-24 hidden md:block"
    />
  </div>

  <div class="grid gap-8 md:gap-4 md:grid-cols-2">
    <div class="space-y-2">
      <h1>Languages</h1>
      <div class="languages">
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg"
          alt="TypeScript"
        />
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg"
          alt="JavaScript"
        />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/php/php-original.svg" alt="PHP" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" alt="C++" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" alt="C#" />
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/rust/rust-plain.svg" alt="Rust" />
      </div>
    </div>
    <div class="space-y-2">
      <h1>Technologies</h1>
      <div class="languages">
        <img
          class="dark:invert"
          src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/svelte/svelte-plain.svg"
          alt="Svelte"
        />
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg"
          alt="Postgres"
        />
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg"
          alt="NodeJs"
        />
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cmake/cmake-original.svg"
          alt="cmake"
        />
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg"
          alt="Visual Studio Code"
        />
        <img
          src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/visualstudio/visualstudio-plain.svg"
          alt="Visual Studio"
        />
        <img
          src="Ida.png"
          alt="IDA Pro"
        />
      </div>
    </div>
  </div>

  <div class="space-y-2 relative overflow-x-hidden">
    <div>
      <h1>Projects</h1>
      <p class="text-sm">
        Various projects made with different technologies.
      </p>
    </div>
    <div class="projects grid gap-4 md:grid-cols-2">
      <Project title="edk2-cmake" href="https://github.com/dllcrt0/edk2-cmake" thumbnail="edk2cmake.webp">
        Project to use EDK-II and edk-2 with cmake.
      </Project>

      <Project title="cod-deob" href="https://github.com/dllcrt0/cod-deob" thumbnail="cod-deob.webp">
        Project to remote code flow obfuscation in a variety of Call of Duty titles.
      </Project>

      <Project title="py-assembler" href="https://github.com/dllcrt0/py-assembler" thumbnail="py-assembler.webp">
        Project to assemble and disassemble x86/x64 assembly using gcc and objdump.
      </Project>

      <Project title="x360-challenge-api" href="https://github.com/dllcrt0/x360-challenge-api" thumbnail="x360-challenge-api.webp">
        Project to handle hypervisor and supervisor security challenges on Xbox360.
      </Project>

      <Project title="bedaisy-reversal" href="https://github.com/dllcrt0/bedaisy-reversal" thumbnail="bedaisy-reversal.webp">
        Project showing devirtualized pseuedo-code from popular anti-cheat BattlEye's kernel driver BEDaisy.sys.
      </Project>

      <Project title="battleye-decryption" href="https://github.com/dllcrt0/battleye-decryption" thumbnail="battleye-decryption.webp">
        Project that decrypts multiple BattlEye packets from BEService to/from BEDaisy.
      </Project>
    </div>
  </div>

  <p>&copy; {new Date().getFullYear()} dllcrt0</p>
</div>
