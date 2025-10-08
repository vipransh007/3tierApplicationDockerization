# step-1 ---- CALLNG FROM BASE IMAGE USING FROM KEYWORD
FROM node:18.9.1

# Step-2 --- spcifyng which work directory we are using
WORKDIR /app

# step-3 ---- Copyin all the required files from our package.json
COPY package.json .
# FROM our package.json we will copy everything into our main directory HERE
# from PACKAGE.JSON ------>> . (Here in this)

#Step-4 ----- The run command which will help in running
RUN npm install
# This command ensures that this Command will run first and will 
# Install all the dependencies here itself

# Step-5 ---- After installing the required packages now we will copy the complete source code
COPY . .

# Step-6 --- Now we neeed to give access to the port basically exposing hte port
EXPOSE 5173

# Step-7 --- Now Simply running a CMD command we can also use ENTRYPOINT Command
RUN ["npm" , "run", "dev"]
