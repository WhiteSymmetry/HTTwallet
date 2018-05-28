**1. Clone wallet sources**

```
git clone https://github.com/WhiteSymmetry/HTTwallet.git
```

**2. Modify `CryptoNoteWallet.cmake`**
 
```
set(CN_PROJECT_NAME "HiperTeknolojiToken")
set(CN_CURRENCY_DISPLAY_NAME "HiperTeknoloji Token")
set(CN_CURRENCY_TICKER "HTT")
```

**3. Set symbolic link to coin sources at the same level as `src`. For example:**

```
ln -s ../HiperTeknolojiToken HiperTeknolojiToken
```

Alternative way is to create git submodule:

```
git submodule add https://github.com/WhiteSymmetry/HiperTeknolojiToken.git HiperTeknolojiToken
```

Replace URL with git remote repository of your coin.

**4. Build**

```
mkdir build && cd build && cmake .. && make
```
