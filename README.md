# yii2-rubytag-devenv

A sample of developing composer packages locally (and is used for deveoping yii2-rubytag extension).

## Setup environtment

1. Create an yii2 app skeleton (I use basic template).
2. Edit app *composer.json*, add the code below to *repositories* part
    ```json
    {
      "type": "path",
      "url": "../../yii2-rubytag",
      "options": {
          "symlink": true
      }
    }
    ```
3. Run composer require to create link of the library to vendor folder.
   ```shell
   cd src
   composer require umbalaconmeogia/yii2-rubytag @dev
   ```

## References

* [Developing composer packages locally](https://johannespichler.com/developing-composer-packages-locally/)