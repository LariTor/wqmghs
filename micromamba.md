## [Micromamba](https://mamba.readthedocs.io/en/latest/user_guide/micromamba.html)
<details>
<summary><b>Instalación</b></summary>
install using paru y fish

``` paru -S micromamba ```

init 

```micromamba shell init --shell=fish --prefix=~/mamba >> .config/fish/config.fish```

vamos a .config.fish y borramos el excedente[^1].
deberiamos ver esto:
```
# >>> mamba initialize >>>
# !! Contents within this block are managed by 'mamba init' !!
set -gx MAMBA_EXE "/usr/bin/micromamba"
set -gx MAMBA_ROOT_PREFIX "~/.config/mamba"
$MAMBA_EXE shell hook --shell fish --root-prefix $MAMBA_ROOT_PREFIX | source
# <<< mamba initialize <<<
```
y hacemos en home:
```mv mamba/ .config/  ```

yo voy a ponerle un alias en fish para que cada vez que diga conda, sea micromamba:
``` alias conda micromamba ```

[^1]: (Modifying RC file "/home/user/.config/fish/config.fish"
Generating config for root prefix "/home/user/mamba"
Setting mamba executable to: "/usr/bin/micromamba"
Adding (or replacing) the following in your "/home/user/.config/fish/config.fish" file)

</details>

<details>
<summary><b>Primeros pasos</b></summary>
  
activar enviroment base:
```micromamba activate```

crear enviroment:
```micromamba create -n $env_name$```

activar enviroment custom:
```micromamba activate $env_name$ ```

ahora hacemos:

```conda install -c conda-forge $packacge$```

```micromamba config append channels conda-forge```
</details>
