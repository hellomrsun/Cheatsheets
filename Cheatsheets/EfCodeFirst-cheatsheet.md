# Entity Framework Code First cheat sheet



#### Activate entity framework code first migrations
```bash
> Enable-Migrations
```

#### Revert the first migration
```bash
> Update-Database -target:0
```

#### Generate migration file for newly added models
```bash
> Add-Migration {MigrationName}
```

#### Update database with version
```bash
> Update-Database -TargetMigration {MigrationName}
```

#### Generate migration script for new migration or old migration rollback:
```bash
> Update-Database -TargetMigration {MigrationName} -script
```
