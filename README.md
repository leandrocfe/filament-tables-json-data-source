# How to consume an external API with Filament Tables

Sometimes you want to use Filament Tables, but without dealing with a database table.
This example will allow you to determine the rows for the model getting data from an external source (JSON API).

Data reference: https://dummyjson.com/products

![screenshot](https://raw.githubusercontent.com/leandrocfe/filament-tables-json-data-source/master/screenshots/example.jpg)

## Installation

Clone the repository:

```bash
git clone https://github.com/leandrocfe/filament-tables-json-data-source.git
```

Switch to the repo folder:

```bash
cd filament-tables-json-data-source
```

Create a new MySQL database called `filament_tables_json_data_source`. Copy the example env file and set the database connection:

```bash
cp .env.example .env
```

```bash
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=filament_tables_json_data_source
DB_USERNAME=YOUR_USERNAME
DB_PASSWORD=YOUR_PASSWORD
```

You may run the following commands in your terminal:

```bash
composer install
php artisan migrate
```

You may create a new user account using:

```bash
php artisan make:filament-user
```

## Usage

After the project has been built, start Laravel's local development server using the Laravel's Artisan CLI serve command:

```bash
php artisan serve
```

Once you have started the Artisan development server, your application will be accessible in your web browser at [http://localhost:8000/admin](http://localhost:8000/admin).

Visit your Product Resource at /admin/products to try it! Hope you enjoy!

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
