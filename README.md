## Tech Stack

- **Next JS**
- **Tailwind**
- **Redux Toolkit**
- **Redux Toolkit Query**
- **Material UI Data Grid**
- **Node.js**
- **Prisma**
- **AWS EC2**
- **AWS RDS**
- **AWS API Gateway**
- **AWS Amplify**
- **AWS S3**

## Installation Steps

1. **Clone the repository**:
    ```bash
    git clone [git-url]
    cd inventory-management
    ```

2. **Install dependencies for both client and server**:
    ```bash
    # Client setup
    cd client
    npm i
    cd ..

    # Server setup
    cd server
    npm i
    ```

3. **Set up the database**:
    ```bash
    npx prisma generate
    npx prisma migrate dev --name init
    npm run seed
    ```

4. **Configure environment variables**:
    - For server settings, configure the `.env` file:
        ```plaintext
        PORT=your-port
        DATABASE_URL=your-database-url
        ```
    - For client settings, configure the `.env.local` file:
        ```plaintext
        NEXT_PUBLIC_API_BASE_URL=your-api-base-url
        ```

5. **Run the project**:
    Run this command in both client and server environments
    ```bash
    npm run dev
    ```


### Additional Resources

- [Data model diagram](https://drawsql.app/teams/team-3023/diagrams/56-inventorymanagement)
- [Prisma schema file](https://github.com/ed-roh/inventory-management/blob/master/server/prisma/schema.prisma)
- [AWS commands](https://github.com/ed-roh/inventory-management/blob/master/server/aws-ec2-instructions.md)
