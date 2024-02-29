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
  sudo pacman -S  base linux-firmware git htop btop waybar wlroots hyprland qt5-wayland qt6-wayland foot allacritty dunst rofi mesa vulkan-intel lib32-mesa ntfs-3g xdg-desktop-portal-wlr xdg-desktop-portal-hyprland neovim  hyprpaper wl-clipboard  python firefox udisks2 tlp ranger  translate-shell networkmanager zsh
  ```


 dhcpcd 
systemctl enable dhcpcd ->>>>>>>>>>>>>>>>> вместо networkmanager

 <a id="#второй-элемен"></a>

## Установка AUR

  ```
  pacman -S --needed git base-devel && git clone https://aur.archlinux.org/yay-bin.git && cd yay-bin && makepkg -si
  ```
 


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