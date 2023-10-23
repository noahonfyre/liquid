<template>
  <div class="flex flex-col gap-8 w-screen h-screen bg-white p-12">
    <PreviewSection heading="Headings">
      <LiquidHeading large>Large Heading</LiquidHeading>
      <LiquidHeading normal>Normal Heading</LiquidHeading>
      <LiquidHeading small>Small Heading</LiquidHeading>
    </PreviewSection>

    <PreviewSection heading="Buttons">
      <LiquidButton primary color="default">Primary Button</LiquidButton>
      <LiquidButton primary color="yellow">Warn Button</LiquidButton>
      <LiquidButton primary color="red">Severe Button</LiquidButton>
      <LiquidButton secondary>Secondary Button</LiquidButton>
      <LiquidButton tertiary>Tertiary Button</LiquidButton>
    </PreviewSection>

    <PreviewSection heading="Inputs">
      <LiquidInput placeholder="Default Input"></LiquidInput>
      <LiquidInput placeholder="Input with icon">
        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
          <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z" />
        </svg>
      </LiquidInput>
    </PreviewSection>

    <PreviewSection heading="General components">
      <LiquidText>Text component</LiquidText>
      <LiquidLink target="https://google.com">Link component</LiquidLink>
    </PreviewSection>

    <PreviewSection heading=""></PreviewSection>
  </div>
</template>
