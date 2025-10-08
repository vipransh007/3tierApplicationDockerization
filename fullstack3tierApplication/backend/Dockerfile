# Step-1 : importing image
FROM node:18.9.1

# calling the workdirectory 
WORKDIR /app

# COPYING THE REQUIREMENTS FROM PACKAGE.JSON
RUN npm install

# Copy the source code here after installing 
COPY . .

# Exposing the Ports
EXPOSE 5050

CMD ["npm" , "start"]