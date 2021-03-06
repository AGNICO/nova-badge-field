# Laravel Nova Badge Field

Simple Laravel Nova Badge field.  It extends the `Select` field and allows a simple mapping of colors to values to display a "Badge" in the index.

### Details Page

![details page select](https://cdn-pro.dprcdn.net/files/acc_465612/S5MDqi)

### Index 

![index badge](https://cdn-pro.dprcdn.net/files/acc_465612/gibgjD)

## Installation

You can install the package in to a Laravel app that uses [Nova](https://nova.laravel.com) via composer:

```bash
composer require timothyasp/nova-badge-field
```

## Usage


```
Badge::make('Field')
   ->options($options)
   ->colors([
      'option1' => '#ffffff',
      'option2' => '#000000'
   ]);
```

If you want to set the text color of the badge, set the color attribute on the option.  If there isn't an option set, it defaults to setting the background color and the text color is set to a contrasting white/black color based on the brightness of the background. 
```
Badge::make('Field')
   ->options($options)
   ->colors([
      'option1' => [
          'background' => '#ffffff',
          'color' => '#000000'
      ],
      'option2' => '#000000'
   ]);
```


## Credits

- [Timothy Asp](https://github.com/timothyasp)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
