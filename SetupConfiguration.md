### Database Connections
1. Add a connection string (keep it private) in user secrets
    - PostgreSql : Host=localhost;Port=5432;Database=MyDb;Username=myuser;Password=mypassword;
2. Add the service to connect to database in Program.cs
    - builder.Services.AddDbContext<ApplicationDbContext>(options =>
			options.UseNpgsql(builder.Configuration.GetConnectionString("DefaultConnection")));
3. In package console
    - add-migration <Migration Name>
    - update database
    - remove-migration

### Swagger Congifuration
- Install the required packages
- In Program.cs
    - builder.Services.AddEndpointsApiExplorer();
		builder.Services.AddSwaggerGen();

		if (app.Environment.IsDevelopment())
		{
			app.UseSwagger();
			app.UseSwaggerUI();
		}
- In Launch Settings.json
    - "launchBrowser": true,
	    "applicationUrl": "https://localhost:7119;http://localhost:5110",
		"launchUrl": "swagger",

### Logging Configuration
- On Hold
