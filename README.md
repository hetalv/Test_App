# Test_App
Please create a table in Sql DB with attached script
SET ANSI_NULLS ON
GO

SET QUOTED_IDENTIFIER ON
GO

CREATE TABLE [dbo].[Contacts](
	[Id] [numeric](18, 0) IDENTITY(1,1) NOT NULL,
	[FirstName] [varchar](50) NOT NULL,
	[LastName] [varchar](50) NOT NULL,
	[Email] [varchar](50) NOT NULL,
	[PhoneNumber] [varchar](50) NULL,
	[Status] [bit] NOT NULL
) ON [PRIMARY]
GO

Now connect to your local db, change the connection string in appsetting.json file of the project and you can run the application.
