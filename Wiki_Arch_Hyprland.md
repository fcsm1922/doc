 **Содержание:**

 - [Установка базовых пакетов Arch Linux](#первый-элемент)

 - [Установка AUR](#второй-элемент)

 - [Second Item](#третий-элемент)

 - [Работа с архивами](#четвертый-элемент)

 - [Монтирование дисков](#пятный-элемент)

 <!-- headings -->

 <a id="первый-элемент"></a>

## Установка базовых пакетов Arch Linux

Здесь будет содержаться как установить Arch linux с минимальным колличеством пакетов на wayland
  ```
  sudo pacman -S linux-firmware git htop btop waybar wlroots hyprland qt5-wayland qt6-wayland foot alacritty dunst rofi ntfs-3g xdg-desktop-portal-wlr xdg-desktop-portal-hyprland neovim  hyprpaper wl-clipboard  firefox udisks2 tlp ranger translate-shell networkmanager zsh lxqt-policykit sof-firmware pipewire-pulse wireplumber
  ```
 
 `reflector` - программа для отсортировки зеркал для скачивания пакетов


`mesa vulkan-intel intel-ucode`   - дрова для уставновки на реальное железо
`vulkan-virtio` - для виртуальных машин
`vulkan-headers`
`mesa-utils`
`lib32-mesa`

 <a id="#второй-элемен"></a>

## Установка AUR

  ```
  pacman -S git clone https://aur.archlinux.org/yay-bin.git && cd yay-bin && makepkg -si
  ```
 
 `git clone https://github.com/fcsm1922/doc` - мой репозиторий



 <a id="третий-элемент"></a>

## Second Item



 <a id="четвертый-элемент"></a>

## Работа с архивами

 ### ZIP - архивы

1. Установка пакета `unzip`

  ```
  sudo pacman -S unzip
  ```
2. Извлечь данные из ZIP-файла
  ```
  unzip filename.zip
  ```
> Файл будет извлечен в тот же каталог, где находится ZIP-файл
3. Распаковать ZIP-файл в другой каталог 
  ```
  unzip filename.zip -d /path/of/directory
  ```
 
 ### RAR - архивы

 <a id="пятый-элемент"></a>

 ## Монтирование дисков

### VS-Code
<br>

1. Сначала устанавливаем `Electron27` из исходников

    ```
    yay -S electron27-bin
    ```
2. Затем устанавливаем `VS-code`

    ```
    yay -S  visual-studio-code-bin



    Подключение multilib

sudo micro /etc/pacman.conf

необходимо раскоментировать вот это:
[multilib]
Include = /etc/pacman.d/mirrorlist