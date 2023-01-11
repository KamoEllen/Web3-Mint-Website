# Web3-Mint-Website
npx create react-app full-mint-website
npm i -D hardhat
npx hardhat 
-basic sample project , enter *4
npm i @oppenzeppelin/contracts
npm install @chakra-ui/react @emotion/react @emotion/styled framer-motion
app.text.js,logo.svg,reportWe.js = delete
in index.js , delete line 5 'import reportwe' , line 13-15
go to app.js , delete all in header and line 1 'logo.svg'
contracts greater.sol file, delete it , , replace it with file SpiderFunkNFT.sol



import * as React from 'react'

// 1. import `ChakraProvider` component
import { ChakraProvider } from '@chakra-ui/react'

function App() {
  // 2. Wrap ChakraProvider at the root of your app
  return (
    <ChakraProvider>
      <TheRestOfYourApplication />
    </ChakraProvider>
  )
}
///
import { ChakraBaseProvider, extendBaseTheme } from '@chakra-ui/react'
// `@chakra-ui/theme` is a part of the base install with `@chakra-ui/react`
import chakraTheme from '@chakra-ui/theme'

const { Button } = chakraTheme.components

const theme = extendBaseTheme({
  components: {
    Button,
  },
})

function App() {
  return (
    <ChakraBaseProvider theme={theme}>
      <Component {...pageProps} />
    </ChakraBaseProvider>
  )
}
